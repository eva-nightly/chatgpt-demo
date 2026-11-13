# Module: src

Defines global TypeScript types and environment variable declarations for the chat application, including chat message structures, error schemas, and OpenAI configuration variables.

## Key files
- `src/env.d.ts`: Declares typed environment variables for Astro client and OpenAI configuration (such as API keys, base URLs, proxies, model selection, and message history limits).
- `src/types.ts`: Exports core TypeScript interfaces for chat conversation messages (ChatMessage) and error responses (ErrorMessage).

## Public interface
- interface ChatMessage { role: 'system' | 'user' | 'assistant'; content: string }
- interface ErrorMessage { code: string; message: string }
- interface ImportMetaEnv
- interface ImportMeta

## Dependencies
- astro/client

## AI touchpoints [AI]
- `src/env.d.ts`
- `src/types.ts`

## Where the code disagrees with the stack profile
- `src/env.d.ts`: The stack states the repository uses Next.js route handlers, but env.d.ts references Astro client types (astro/client) and Vite/Astro ImportMetaEnv.

## Open questions
- _none_

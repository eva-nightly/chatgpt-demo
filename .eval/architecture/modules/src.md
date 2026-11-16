# Module: src

Defines core TypeScript type declarations and environment variable definitions for the chat application, including chat message structures, error responses, and configuration keys.

## Key files
- `src/types.ts`: Exports shared TypeScript interfaces for chat messages (ChatMessage) and error responses (ErrorMessage).
- `src/env.d.ts`: Provides TypeScript definitions for client environment variables (ImportMetaEnv) and references Astro client types.

## Public interface
- interface ChatMessage
- interface ErrorMessage
- interface ImportMetaEnv
- interface ImportMeta

## Dependencies
- astro/client

## AI touchpoints [AI]
- `src/types.ts`
- `src/env.d.ts`

## Where the code disagrees with the stack profile
- `src/env.d.ts`: The stack states the project uses Next.js route handlers, but the type definition references Astro via astro/client and ImportMetaEnv.

## Open questions
- _none_

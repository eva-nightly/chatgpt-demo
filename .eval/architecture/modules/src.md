# Module: src

Provides shared TypeScript definitions for environment variables, chat message payloads, and error representations used across the chat application.

## Key files
- `src/env.d.ts`: Declares client typing and the ImportMetaEnv interface for configuration variables including API keys and base URLs.
- `src/types.ts`: Defines ChatMessage and ErrorMessage data structures for LLM interaction and error handling.

## Public interface
- export interface ChatMessage
- export interface ErrorMessage
- interface ImportMetaEnv
- interface ImportMeta

## Dependencies
- astro/client

## AI touchpoints [AI]
- `src/types.ts`
- `src/env.d.ts`

## Where the code disagrees with the stack profile
- `src/env.d.ts`: The stack describes Next.js route handlers and server code, but the code references Astro client types (astro/client) and ImportMetaEnv.

## Open questions
- _none_

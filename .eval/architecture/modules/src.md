# Module: src

Provides core TypeScript type definitions and environment variable interfaces for chat messaging, error handling, and OpenAI-compatible configuration.

## Key files
- `src/env.d.ts`: Declares typed environment variables for OpenAI API connection details, proxies, model names, site passwords, and Astro client types.
- `src/types.ts`: Defines core data models for conversation turns (ChatMessage) and API/provider errors (ErrorMessage).

## Public interface
- interface ChatMessage
- interface ErrorMessage
- interface ImportMetaEnv
- interface ImportMeta

## Dependencies
- astro/client

## AI touchpoints [AI]
- `src/env.d.ts`
- `src/types.ts`

## Where the code disagrees with the stack profile
- `src/env.d.ts`: The environment type definitions reference 'astro/client' indicating an Astro framework rather than Next.js route handlers.

## Open questions
- _none_

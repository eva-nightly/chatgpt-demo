# Module: src

Provides core TypeScript type definitions and environment variable interfaces for the chat interface, including message structures, error schemas, and OpenAI/runtime configuration settings.

## Key files
- `src/env.d.ts`: Defines typing for Astro client environment variables including OpenAI API keys, base URLs, model selection, proxy settings, site passwords, and history message limits.
- `src/types.ts`: Defines data structures for chat messages (system, user, assistant roles) and error representations.

## Public interface
- interface ChatMessage { role: 'system' | 'user' | 'assistant'; content: string; }
- interface ErrorMessage { code: string; message: string; }
- interface ImportMetaEnv { readonly OPENAI_API_KEY: string; readonly HTTPS_PROXY: string; readonly OPENAI_API_BASE_URL: string; readonly HEAD_SCRIPTS: string; readonly PUBLIC_SECRET_KEY: string; readonly SITE_PASSWORD: string; readonly OPENAI_API_MODEL: string; readonly PUBLIC_MAX_HISTORY_MESSAGES: string; }

## Dependencies
- astro/client

## AI touchpoints [AI]
- `src/env.d.ts`
- `src/types.ts`

## Where the code disagrees with the stack profile
- `src/env.d.ts`: The stack states the project is built on Next.js, but the type definitions reference Astro client types (astro/client) and Vite/Astro-style ImportMetaEnv.

## Open questions
- _none_

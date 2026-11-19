# Module: src/pages [AI]

Provides Astro API route handlers for authenticating site passwords and streaming chat completions from an OpenAI-compatible API.

## Key files
- `src/pages/api/auth.ts`: Handles password validation requests against the configured site password list.
- `src/pages/api/generate.ts`: Handles chat generation requests, validates request signatures and passwords, forwards payloads to the OpenAI-compatible chat completions endpoint, and returns streamed responses.

## Public interface
- post (in src/pages/api/auth.ts)
- post (in src/pages/api/generate.ts)

## Dependencies
- astro
- undici
- @/utils/openAI
- @/utils/auth

## AI touchpoints [AI]
- `src/pages/api/generate.ts`

## Where the code disagrees with the stack profile
- `src/pages/api/auth.ts`: The API routes are Astro endpoints using APIRoute and import.meta.env, not Next.js route handlers.

## Open questions
- _none_

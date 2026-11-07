# Module: src/pages [AI]

Provide server-side API endpoints for password authentication and streaming chat completions through an OpenAI-compatible API.

## Key files
- `src/pages/api/auth.ts`: Handles password validation requests against configured site passwords
- `src/pages/api/generate.ts`: Validates request signature and password, forwards conversation messages to OpenAI chat completions endpoint, and returns the streamed response

## Public interface
- POST /api/auth
- POST /api/generate

## Dependencies
- astro
- undici
- @/utils/openAI
- @/utils/auth

## AI touchpoints [AI]
- `src/pages/api/generate.ts`

## Where the code disagrees with the stack profile
- `src/pages/api/auth.ts`: The stack states the project uses Next.js route handlers and Next.js API routes, but the files use Astro APIRoute handlers (import type { APIRoute } from 'astro') and Astro environment variables (import.meta.env).

## Open questions
- _none_

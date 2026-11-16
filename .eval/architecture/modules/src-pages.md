# Module: src/pages [AI]

Provides server-side API endpoints for password authentication and streaming chat completion generation via OpenAI-compatible endpoints.

## Key files
- `src/pages/api/auth.ts`: Validates the site password submitted in request bodies against the SITE_PASSWORD environment variable.
- `src/pages/api/generate.ts`: Verifies passwords and request signatures, forwards chat completion requests to the configured OpenAI-compatible API base URL, and returns a parsed streaming response.

## Public interface
- export const post: APIRoute (src/pages/api/auth.ts)
- export const post: APIRoute (src/pages/api/generate.ts)

## Dependencies
- astro
- undici
- @/utils/openAI
- @/utils/auth

## AI touchpoints [AI]
- `src/pages/api/generate.ts`

## Where the code disagrees with the stack profile
- `src/pages/api/auth.ts`: The server endpoints are Astro API routes using Astro's APIRoute type and export const post, rather than Next.js route handlers.

## Open questions
- _none_

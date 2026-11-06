# Module: src/pages [AI]

Provides server-side Astro API endpoints for authenticating user site passwords and forwarding chat completion requests to OpenAI-compatible APIs with streaming responses.

## Key files
- `src/pages/api/auth.ts`: Handles password verification requests against configured site passwords.
- `src/pages/api/generate.ts`: Validates request payload, password, and signature, and proxies chat completion requests to the OpenAI-compatible API endpoint.

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
- `src/pages/api/auth.ts`: The scan indicated Next.js API route handlers, but the endpoints are implemented using Astro APIRoute handlers (importing APIRoute from 'astro' and accessing import.meta.env).

## Open questions
- _none_

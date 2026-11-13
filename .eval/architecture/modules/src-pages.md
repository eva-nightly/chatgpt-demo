# Module: src/pages [AI]

Provide server-side API endpoints for password authentication and streaming AI chat completions via an OpenAI-compatible API.

## Key files
- `src/pages/api/auth.ts`: API endpoint for validating user-supplied site passwords against configured site password lists.
- `src/pages/api/generate.ts`: API endpoint for validating request signatures, passwords, and message payloads, forwarding requests to the OpenAI-compatible chat completions endpoint, and returning a streaming response.

## Public interface
- POST /api/auth (post: APIRoute)
- POST /api/generate (post: APIRoute)

## Dependencies
- astro
- undici
- @/utils/openAI
- @/utils/auth

## AI touchpoints [AI]
- `src/pages/api/generate.ts`

## Where the code disagrees with the stack profile
- `src/pages/api/auth.ts`: The stack describes the server code as Next.js route handlers, but the files implement Astro API endpoints using APIRoute from 'astro'.

## Open questions
- _none_

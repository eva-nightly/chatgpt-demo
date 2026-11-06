# Module: src/utils

Provide utility functions for request signature generation/verification and OpenAI-compatible API payload formatting and SSE stream parsing.

## Key files
- `src/utils/auth.ts`: Generates and verifies SHA-256 signatures for authenticating chat requests using timestamps, message content, and secret keys
- `src/utils/openAI.ts`: Builds request payloads for OpenAI chat completions and parses Server-Sent Events (SSE) streaming responses into a readable text stream

## Public interface
- generateSignature(payload: AuthPayload): Promise<string>
- verifySignature(payload: AuthPayload, sign: string): Promise<boolean>
- model: string
- generatePayload(apiKey: string, messages: ChatMessage[], temperature: number): RequestInit & { dispatcher?: any }
- parseOpenAIStream(rawResponse: Response): Response

## Dependencies
- eventsource-parser
- js-sha256
- @/types

## AI touchpoints [AI]
- `src/utils/openAI.ts`

## Where the code disagrees with the stack profile
- `src/utils/auth.ts`: Files use Vite/Astro-style environment variables ('import.meta.env.PUBLIC_SECRET_KEY' and 'import.meta.env.OPENAI_API_MODEL') rather than standard Next.js 'process.env'.

## Open questions
- In src/utils/auth.ts, the timestamp freshness check (checking if t is within 5 minutes) is commented out, leaving signature verification vulnerable to replay attacks.

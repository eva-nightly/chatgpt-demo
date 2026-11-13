# Module: src/utils

Provide utility functions for request signing/verification and OpenAI-compatible API interaction, including request payload construction and SSE response stream parsing.

## Key files
- `src/utils/auth.ts`: Generates and verifies SHA-256 signatures for authenticating requests using timestamp, last message, and a secret key.
- `src/utils/openAI.ts`: Defines default model configuration, builds chat completion request payloads, and parses streaming Server-Sent Events (SSE) from OpenAI-compatible endpoints into a readable stream.

## Public interface
- generateSignature(payload: AuthPayload): Promise<string>
- verifySignature(payload: AuthPayload, sign: string): Promise<boolean>
- model: string
- generatePayload(apiKey: string, messages: ChatMessage[], temperature: number): RequestInit & { dispatcher?: any }
- parseOpenAIStream(rawResponse: Response): Response

## Dependencies
- js-sha256
- eventsource-parser
- @/types

## AI touchpoints [AI]
- `src/utils/openAI.ts`

## Where the code disagrees with the stack profile
- `src/utils/auth.ts`: The environment uses Vite/Astro-style `import.meta.env` (e.g. `import.meta.env.PUBLIC_SECRET_KEY`, `import.meta.env.OPENAI_API_MODEL`) rather than Next.js standard `process.env`.

## Open questions
- Timestamp expiration check in verifySignature is commented out; is request replay protection intentionally disabled?
- Why does openAI.ts access import.meta.env instead of process.env if running in a Node/Next.js environment?

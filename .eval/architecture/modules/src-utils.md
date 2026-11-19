# Module: src/utils

Provides utility functions for request authentication signature hashing/verification and for constructing and parsing OpenAI-compatible streaming chat completion requests.

## Key files
- `src/utils/auth.ts`: Generates and verifies cryptographic signatures for request payload authentication using Web Crypto or js-sha256.
- `src/utils/openAI.ts`: Configures model defaults, builds request payloads for OpenAI-compatible streaming endpoints, and parses SSE stream chunks into a readable text stream.

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
- `src/utils/auth.ts`: The files use import.meta.env (typical for Vite/Astro) instead of process.env, contradicting the scan's claim of a standard Next.js environment.

## Open questions
- Timestamp expiration check in verifySignature is commented out; is request replay protection intentionally disabled?

# Module: src/utils

Provides utility functions for request authorization hashing/signature verification and formatting OpenAI chat completion request payloads and SSE streaming responses.

## Key files
- `src/utils/auth.ts`: Generates and verifies SHA-256 signatures for authenticating chat requests using Web Crypto or js-sha256 fallback.
- `src/utils/openAI.ts`: Constructs OpenAI-compatible API request payloads and parses incoming server-sent event (SSE) streams into text chunk streams.

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
- `src/utils/openAI.ts`: Environment variables are read via import.meta.env rather than process.env expected in standard Next.js setups.

## Open questions
- Timestamp expiration validation in verifySignature is currently commented out; should request age verification be re-enabled?

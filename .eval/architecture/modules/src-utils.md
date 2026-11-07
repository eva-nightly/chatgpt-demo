# Module: src/utils

Provides utility functions for request payload generation and server-sent event (SSE) stream parsing for OpenAI-compatible chat completions, as well as signature generation and verification for request authentication.

## Key files
- `src/utils/openAI.ts`: Defines default LLM model configuration, constructs OpenAI chat completion request payloads with streaming enabled, and transforms raw SSE response streams into readable text streams.
- `src/utils/auth.ts`: Generates and verifies SHA-256 request signatures combining timestamp, message content, and secret key using SubtleCrypto or js-sha256 fallback.

## Public interface
- export const model: string
- export const generatePayload: (apiKey: string, messages: ChatMessage[], temperature: number) => RequestInit & { dispatcher?: any }
- export const parseOpenAIStream: (rawResponse: Response) => Response
- export const generateSignature: (payload: { t: number; m: string }) => Promise<string>
- export const verifySignature: (payload: { t: number; m: string }, sign: string) => Promise<boolean>

## Dependencies
- eventsource-parser
- js-sha256
- @/types

## AI touchpoints [AI]
- `src/utils/openAI.ts`

## Where the code disagrees with the stack profile
- `src/utils/openAI.ts`: Environment variables are loaded using import.meta.env (Vite / Astro standard) rather than process.env typical of Next.js.

## Open questions
- The 5-minute timestamp expiration check in verifySignature is commented out in src/utils/auth.ts, potentially allowing replayed signatures.

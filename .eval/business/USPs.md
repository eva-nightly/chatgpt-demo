# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Minimal single-page streaming chat

A minimal web chat interface: the user types a message on a single page and reads the AI's reply as it streams in.

- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat app: the user types a message and an AI model (via OpenRouter, OpenAI-compatible API) answers in a streaming conversation."
  - `business.md`: "ChatGPT-API Demo is a minimal web chat interface for talking to a large language model."
  - `business.md`: "A single page where a visitor types a message and reads the AI's reply as it streams in."
- **Delivered by:** _no linked components_

## OpenRouter / OpenAI-compatible backend

The AI model is reached through OpenRouter using an OpenAI-compatible API, with the base URL configurable via OPENAI_API_BASE_URL.

- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat app: the user types a message and an AI model (via OpenRouter, OpenAI-compatible API) answers in a streaming conversation."
  - `business.md`: "The AI is reached through OpenRouter using an OpenAI-compatible API (base URL set by OPENAI_API_BASE_URL)."
- **Delivered by:** _no linked components_

## Self-hosted and private by design

Conversations are kept in the browser only; there is no database and no sign-in, making it a simple self-hosted ChatGPT-style page.

- **Sources:**
  - `About_the_organisation.md`: "Developers and curious people who want a simple self-hosted ChatGPT-style chat page."
  - `business.md`: "Conversations are kept in the browser only; there is no database and no sign-in."
  - `business.md`: "Developers and hobbyists who want a simple, self-hosted ChatGPT-style page, and small teams who want a private chat for everyday questions."
- **Delivered by:** _no linked components_

## Open source, small codebase

Released under the MIT license with a small codebase.

- **Sources:**
  - `business.md`: "Open source (MIT), small codebase, last major changes in 2023, so dependencies are old."
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 10 · rule: 0/6 · usp: 0/4
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (10)

- **usp** Minimal single-page streaming chat: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** OpenRouter / OpenAI-compatible backend: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Self-hosted and private by design: The only words that matched a name, path or route are too short to mean one thing (page), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Open source, small codebase: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** Harmless requests must not be refused; unsafe requests are declined politely.: No artifact mentions any of: answ, clearly, correct, declin, good, harmles, politely, question, refus, relevant, request, unsafe, writt.
- **rule** Answers must be correct, relevant to the question, and clearly written.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** Conversations are kept in the browser only; there must be no database and no sign-in.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Replies must start streaming within a couple of seconds.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Errors (e.g. bad key, rate limit) must be explained in plain language; never show a blank screen.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** The AI must be reached via OpenRouter using an OpenAI-compatible API, with the base URL set by OPENAI_API_BASE_URL.: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.

## Gaps

_None. All material was sourced._

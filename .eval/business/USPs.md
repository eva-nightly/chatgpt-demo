# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Streamed replies

A visitor types a message and an AI assistant answers, streamed word by word from an OpenAI-compatible API.

- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat UI where a visitor types messages and an AI assistant replies, streamed from an OpenAI-compatible API via OpenRouter."
  - `about.md`: "A visitor types a message and an AI assistant answers, streamed word by word."
- **Delivered by:** _no linked components_

## Single server route to an OpenAI-compatible API

Requests go to an OpenAI-compatible API (OpenRouter) through one server route.

- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat UI where a visitor types messages and an AI assistant replies, streamed from an OpenAI-compatible API via OpenRouter."
  - `about.md`: "Requests go to an OpenAI-compatible API (OpenRouter) through one server route."
- **Delivered by:**
  - `src/pages/api/generate::post`, matched on route "api" in /api/generate; endpoint "route" in route:/api/generate

## Minimal web chat UI

A minimal web chat interface for talking to a large language model, intended as a demo and self-hosted page.

- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat UI where a visitor types messages and an AI assistant replies, streamed from an OpenAI-compatible API via OpenRouter."
  - `about.md`: "ChatGPT-API Demo is a minimal web chat interface for talking to a large language model."
  - `about.md`: "Developers and hobbyists who want a self-hosted chat page."
- **Delivered by:** _no linked components_

## Visitor-configurable system prompt

The visitor can set a system prompt that shapes the assistant's behaviour.

- **Sources:**
  - `about.md`: "The visitor can set a system prompt that shapes the assistant's behaviour."
- **Delivered by:** _no linked components_

## No database, no sign-in

The conversation stays in the browser; there is no database and no sign-in, making it a simple self-hosted chat page.

- **Sources:**
  - `about.md`: "The conversation stays in the browser; there is no database and no sign-in."
  - `about.md`: "Developers and hobbyists who want a self-hosted chat page."
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 3 of 13 · rule: 2/8 · usp: 1/5
- **Artifacts reached from the business:** 2 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 1 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 1 of 4
- Plugins: 0 of 2

### Linked to nothing (10)

- **usp** Streamed replies: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Minimal web chat UI: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Visitor-configurable system prompt: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **usp** No database, no sign-in: The only words that matched a name, path or route are too short to mean one thing (page), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** Replies must be clear, correct, on topic and follow the conversation so far.: 3 candidate(s) were offered and the model confirmed none of them.
- **rule** The system prompt set by the visitor must be respected by the assistant.: 3 candidate(s) were offered and the model confirmed none of them.
- **rule** Replies are streamed to the visitor word by word.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** The assistant answers the visitor's chat messages as a helpful general assistant.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** Replies must start within a few seconds.: No artifact mentions any of: repli, second, start.
- **rule** The conversation stays in the browser; there is no database and no sign-in.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.

## Gaps

_None. All material was sourced._

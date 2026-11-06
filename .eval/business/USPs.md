# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Minimal, fast web chat with streaming answers

A minimal web chat UI for talking to an AI model, sending messages to an OpenAI-compatible API and streaming the answer back.

- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat UI where people talk to an AI assistant, with streaming answers, through an OpenAI-compatible API."
  - `about-chatgpt-demo.md`: "ChatGPT-API Demo is a minimal web chat interface for talking to an AI model."
  - `about-chatgpt-demo.md`: "Sends the user's messages to an OpenAI-compatible API and streams the answer back."
- **Delivered by:** _no linked components_

## No account, no database

Conversation is kept in the browser; there is no database and no sign-in required.

- **Sources:**
  - `About_the_organisation.md`: "Individuals and small teams who want a simple, fast chat with an AI model, without an account."
  - `about-chatgpt-demo.md`: "Individuals and small teams who want a quick, no-account chat with a model."
  - `about-chatgpt-demo.md`: "Keeps the conversation in the browser; there is no database and no sign-in."
- **Delivered by:** _no linked components_

## Open source and one-command self-hosting

MIT-licensed and can be self-hosted with a single command.

- **Sources:**
  - `about-chatgpt-demo.md`: "It is open source (MIT) and can be self-hosted with one command."
- **Delivered by:** _no linked components_

## Bring your own compatible provider

The owner can point the app at any OpenAI-compatible provider, such as OpenRouter.

- **Sources:**
  - `about-chatgpt-demo.md`: "Lets the owner point it at any compatible provider, such as OpenRouter."
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 8 · rule: 0/4 · usp: 0/4
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (8)

- **usp** Minimal, fast web chat with streaming answers: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** No account, no database: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **usp** Open source and one-command self-hosting: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Bring your own compatible provider: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** Answers must start quickly and read clearly.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** Errors from the AI provider must be explained in plain words.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** A user should never lose their conversation by accident.: No artifact mentions any of: accident, conversation, lose, user.
- **rule** The owner's API key must never reach the browser.: The only words that matched a name, path or route are too short to mean one thing (api), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.

## Gaps

_None. All material was sourced._

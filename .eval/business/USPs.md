# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Minimal, fast chat page with no sign-in

A deliberately minimal web chat interface for talking to a large language model, aimed at people who want a simple, fast chat page without having to sign in.

- **Sources:**
  - `About_the_organisation.md`: "Minimal web UI for ChatGPT."
  - `about.md`: "A minimal web chat interface for talking to a large language model."
  - `about.md`: "Individual people who want a simple, fast chat page without sign-in."
- **Delivered by:** _no linked components_

## Model access through OpenRouter

The AI is reached through OpenRouter via an OpenAI-compatible API, giving ChatGPT-like helpful answers.

- **Sources:**
  - `About_the_organisation.md`: "Answers the visitor's chat messages helpfully, like ChatGPT, through OpenRouter."
  - `about.md`: "The AI is reached through OpenRouter via an OpenAI-compatible API."
- **Delivered by:** _no linked components_

## Streamed answers

Visitors type a message and receive the answer streamed back rather than waiting for a complete response.

- **Sources:**
  - `about.md`: "Visitors type a message and receive a streamed answer."
- **Delivered by:** _no linked components_

## Conversation history stays in the browser

The conversation history is kept in the visitor's browser rather than on a server.

- **Sources:**
  - `about.md`: "The conversation history is kept in the browser."
- **Delivered by:** _no linked components_

## Starting point for developers' own chat apps

The project doubles as a starting point for developers who want to build their own chat application.

- **Sources:**
  - `about.md`: "Developers who want a starting point for their own chat app."
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 12 · rule: 0/7 · usp: 0/5
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (12)

- **usp** Minimal, fast chat page with no sign-in: The only words that matched a name, path or route are too short to mean one thing (page), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Model access through OpenRouter: The only words that matched a name, path or route are too short to mean one thing (api, open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Streamed answers: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Conversation history stays in the browser: No artifact mentions any of: brows, conversation, history, kept, serv, stay, visitor.
- **usp** Starting point for developers' own chat apps: No artifact mentions any of: app, application, build, chat, develop, doubl, point, project, start, want.
- **rule** Answers must be correct, relevant and readable.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** The assistant must follow the system prompt and the conversation context.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** The AI is reached through OpenRouter via an OpenAI-compatible API.: The only words that matched a name, path or route are too short to mean one thing (api, open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** Errors must be shown clearly and must never leave the page blank.: The only words that matched a name, path or route are too short to mean one thing (page), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** Conversation history is kept in the browser.: No artifact mentions any of: brows, conversation, history, kept.
- **rule** Answers are streamed to the visitor.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Visitors can use the chat page without signing in.: The only words that matched a name, path or route are too short to mean one thing (page), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.

## Gaps

_None. All material was sourced._

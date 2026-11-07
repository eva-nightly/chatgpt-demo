# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Minimal single-window chat UI

A deliberately minimal web interface: one chat window where the user types a question and reads the answer, with no account system around it.

- **Sources:**
  - `About_the_organisation.md`: "Minimal web UI for ChatGPT."
  - `about-chatgpt-demo.md`: "ChatGPT-API Demo is a minimal web chat interface for talking to a large language model."
  - `about-chatgpt-demo.md`: "Shows a single chat window where the user types a question and reads a streamed answer."
  - `about-chatgpt-demo.md`: "Developers who want a private chat UI without an account system."
- **Delivered by:** _no linked components_

## Works with any OpenAI-compatible API

The conversation is sent to an OpenAI-compatible API, in this deployment routed through OpenRouter.

- **Sources:**
  - `About_the_organisation.md`: "Individuals and small teams who want a simple self-hosted chat UI for an OpenAI-compatible model."
  - `about-chatgpt-demo.md`: "Sends the conversation to an OpenAI-compatible API, here routed through OpenRouter."
- **Delivered by:** _no linked components_

## Open source and self-hosted

Released under the MIT licence and meant to be self-hosted by individuals and small teams behind their own API key.

- **Sources:**
  - `about-chatgpt-demo.md`: "It is open source (MIT) and meant to be self-hosted by individuals and small teams."
  - `about-chatgpt-demo.md`: "Small teams sharing one deployment behind their own API key."
- **Delivered by:** _no linked components_

## No server-side data storage

There is no database and no sign-in; nothing is stored on the server, giving users a private chat UI.

- **Sources:**
  - `about-chatgpt-demo.md`: "No data is stored on the server: there is no database and no sign-in."
  - `about-chatgpt-demo.md`: "Developers who want a private chat UI without an account system."
- **Delivered by:** _no linked components_

## Streamed answers that don't freeze the UI

Answers arrive quickly and are streamed to the user without the interface freezing.

- **Sources:**
  - `about-chatgpt-demo.md`: "Shows a single chat window where the user types a question and reads a streamed answer."
  - `about-chatgpt-demo.md`: "Answers arrive quickly and stream without freezing."
- **Delivered by:** _no linked components_

## System prompt, clear and export controls

The user can set a system prompt and clear or export the conversation.

- **Sources:**
  - `about-chatgpt-demo.md`: "Lets the user set a system prompt, and clear or export the conversation."
- **Delivered by:** _no linked components_

## Plain-language error handling

Errors from the model provider are explained in plain words rather than leaving a blank screen.

- **Sources:**
  - `about-chatgpt-demo.md`: "Errors from the model provider are explained in plain words, not a blank screen."
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 14 · rule: 0/7 · usp: 0/7
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (14)

- **usp** Minimal single-window chat UI: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Works with any OpenAI-compatible API: The only words that matched a name, path or route are too short to mean one thing (api, open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Open source and self-hosted: The only words that matched a name, path or route are too short to mean one thing (api, open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** No server-side data storage: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **usp** Streamed answers that don't freeze the UI: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** System prompt, clear and export controls: 1 candidate(s) were offered and the model confirmed none of them.
- **usp** Plain-language error handling: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** No data is stored on the server: there is no database and no sign-in.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Errors from the model provider must be explained in plain words, never shown as a blank screen.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Answers must arrive quickly and stream without freezing the UI.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** The assistant stays helpful, honest and on topic, and says so when it does not know.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** The conversation is sent to an OpenAI-compatible API, routed through OpenRouter.: The only words that matched a name, path or route are too short to mean one thing (api, open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** The user must be able to set a system prompt and clear or export the conversation.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** The UI shows a single chat window where the user types a question and reads a streamed answer.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).

## Gaps

_None. All material was sourced._

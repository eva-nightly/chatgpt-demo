# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Minimal web chat UI

A minimal web chat interface for talking to a large language model: visitors open the page, type a question, and get an answer in a chat thread.

- **Sources:**
  - `About_the_organisation.md`: "Minimal web UI for ChatGPT."
  - `about.md`: "ChatGPT-API Demo is a minimal web chat interface for talking to a large language model."
  - `about.md`: "Visitors open the page, type a question, and get a streamed answer in a chat thread."
- **Delivered by:** _no linked components_

## General assistant behaviour

The assistant answers the visitor's chat messages like a general assistant.

- **Sources:**
  - `About_the_organisation.md`: "It answers the visitor's chat messages like a general assistant."
- **Delivered by:** _no linked components_

## No accounts, no database

There is no sign-in and no database; conversations live in the browser, giving a simple, fast chat UI without accounts.

- **Sources:**
  - `about.md`: "There is no sign-in and no database; conversations live in the browser."
  - `about.md`: "Individual developers and curious users who want a simple, fast chat UI without accounts."
- **Delivered by:** _no linked components_

## Streamed answers

Answers are streamed into the chat thread quickly rather than delivered only after completion.

- **Sources:**
  - `about.md`: "Visitors open the page, type a question, and get a streamed answer in a chat thread."
  - `about.md`: "Replies stream quickly and do not cut off mid-sentence."
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 11 · rule: 0/7 · usp: 0/4
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (11)

- **usp** Minimal web chat UI: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** General assistant behaviour: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **usp** No accounts, no database: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **usp** Streamed answers: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Replies must be in the language the visitor wrote in.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** The assistant must admit when it does not know instead of inventing facts; wrong or invented answers presented confidently are unacceptable.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** Replies must stream quickly and must not cut off mid-sentence.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Replies must not ignore a system instruction set by the owner.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Errors must not be shown to the visitor when the model provider is slow or unavailable.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Long conversations must keep context and stay coherent.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** There is no sign-in and no database; conversations live only in the browser.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.

## Gaps

_None. All material was sourced._

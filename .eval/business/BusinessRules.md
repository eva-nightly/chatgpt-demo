# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

Answers must be correct, relevant and readable.

- **Verifiable:** ❌ no
- **Sources:**
  - `About_the_organisation.md`: "Right means a correct, relevant, readable answer that follows the conversation and its instructions."
  - `about.md`: "Answers are correct, relevant and readable."
- **Components:** _no linked components_

### Rule 2

The assistant must follow the system prompt and the conversation context.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "Right means a correct, relevant, readable answer that follows the conversation and its instructions."
  - `about.md`: "The assistant follows the system prompt and the conversation context."
- **Components:** _no linked components_

### Rule 3

The AI is reached through OpenRouter via an OpenAI-compatible API.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "Answers the visitor's chat messages helpfully, like ChatGPT, through OpenRouter."
  - `about.md`: "The AI is reached through OpenRouter via an OpenAI-compatible API."
- **Components:** _no linked components_

### Rule 4

Errors must be shown clearly and must never leave the page blank.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "Errors are shown clearly and never leave the page blank."
- **Components:** _no linked components_

### Rule 5

Conversation history is kept in the browser.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "The conversation history is kept in the browser."
- **Components:** _no linked components_

### Rule 6

Answers are streamed to the visitor.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "Visitors type a message and receive a streamed answer."
- **Components:** _no linked components_

### Rule 7

Visitors can use the chat page without signing in.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "Individual people who want a simple, fast chat page without sign-in."
- **Components:** _no linked components_

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

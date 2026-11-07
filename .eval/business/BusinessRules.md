# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

No data is stored on the server: there is no database and no sign-in.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "No data is stored on the server: there is no database and no sign-in."
- **Components:** _no linked components_

### Rule 2

Errors from the model provider must be explained in plain words, never shown as a blank screen.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "Errors from the model provider are explained in plain words, not a blank screen."
- **Components:** _no linked components_

### Rule 3

Answers must arrive quickly and stream without freezing the UI.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "Answers arrive quickly and stream without freezing."
- **Components:** _no linked components_

### Rule 4

The assistant stays helpful, honest and on topic, and says so when it does not know.

- **Verifiable:** ❌ no
- **Sources:**
  - `about-chatgpt-demo.md`: "The assistant stays helpful, honest and on topic, and says so when it does not know."
- **Components:** _no linked components_

### Rule 5

The conversation is sent to an OpenAI-compatible API, routed through OpenRouter.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "Sends the conversation to an OpenAI-compatible API, here routed through OpenRouter."
- **Components:** _no linked components_

### Rule 6

The user must be able to set a system prompt and clear or export the conversation.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "Lets the user set a system prompt, and clear or export the conversation."
- **Components:** _no linked components_

### Rule 7

The UI shows a single chat window where the user types a question and reads a streamed answer.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "Shows a single chat window where the user types a question and reads a streamed answer."
- **Components:** _no linked components_

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

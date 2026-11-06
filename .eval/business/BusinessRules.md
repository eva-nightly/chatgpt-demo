# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

Answers must start quickly and read clearly.

- **Verifiable:** ❌ no
- **Sources:**
  - `about-chatgpt-demo.md`: "Answers must start quickly and read clearly."
- **Components:** _no linked components_

### Rule 2

Errors from the AI provider must be explained in plain words.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "Errors from the AI provider must be explained in plain words."
- **Components:** _no linked components_

### Rule 3

A user should never lose their conversation by accident.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "A user should never lose their conversation by accident."
- **Components:** _no linked components_

### Rule 4

The owner's API key must never reach the browser.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "The owner's API key must never reach the browser."
- **Components:** _no linked components_

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

# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

Replies should be helpful, accurate, on-topic, follow what the user asked, and stream without errors.

- **Verifiable:** ❌ no
- **Sources:**
  - `About_the_organisation.md`: "Right means a helpful, accurate, on-topic reply that follows what the user asked, streamed without errors."
- **Components:** _no linked components_

### Rule 2

Explain errors, such as a bad key or slow model, in plain words.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "Errors, such as a bad key or a slow model, should be explained in plain words."
- **Components:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 4 · rule: 0/2 · usp: 0/2
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (4)

- **usp** Minimal web chat interface: 1 candidate(s) were offered and the model confirmed none of them.
- **usp** Streaming AI answers: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Replies should be helpful, accurate, on-topic, follow what the user asked, and stream without errors.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** Explain errors, such as a bad key or slow model, in plain words.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.

## Gaps

_None. All material was sourced._

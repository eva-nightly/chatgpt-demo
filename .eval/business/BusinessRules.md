# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

Replies must be clear, correct, on topic and follow the conversation so far.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "Right means a clear, correct, on-topic reply that follows the conversation and the system prompt, and an error message instead of a crash when the model fails."
  - `about.md`: "Replies are correct, on topic and follow the conversation so far."
- **Components:** _no linked components_

### Rule 2

The system prompt set by the visitor must be respected by the assistant.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "Right means a clear, correct, on-topic reply that follows the conversation and the system prompt, and an error message instead of a crash when the model fails."
  - `about.md`: "The system prompt is respected."
  - `about.md`: "The visitor can set a system prompt that shapes the assistant's behaviour."
- **Components:** _no linked components_

### Rule 3

When the model fails or times out, the visitor must see a clear error message, not a crash or blank page.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "Right means a clear, correct, on-topic reply that follows the conversation and the system prompt, and an error message instead of a crash when the model fails."
  - `about.md`: "When the model fails or times out, the visitor sees a clear error, not a blank page."
- **Components:**
  - `src/components/ErrorMessageItem::ErrorMessageItem`, matched on name "error" in ErrorMessageItem; name "message" in ErrorMessageItem

### Rule 4

Replies are streamed to the visitor word by word.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat UI where a visitor types messages and an AI assistant replies, streamed from an OpenAI-compatible API via OpenRouter."
  - `about.md`: "A visitor types a message and an AI assistant answers, streamed word by word."
- **Components:** _no linked components_

### Rule 5

All model requests go to an OpenAI-compatible API (OpenRouter) through a single server route.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat UI where a visitor types messages and an AI assistant replies, streamed from an OpenAI-compatible API via OpenRouter."
  - `about.md`: "Requests go to an OpenAI-compatible API (OpenRouter) through one server route."
- **Components:**
  - `src/pages/api/generate::post`, matched on route "api" in /api/generate; endpoint "route" in route:/api/generate

### Rule 6

The assistant answers the visitor's chat messages as a helpful general assistant.

- **Verifiable:** ❌ no
- **Sources:**
  - `About_the_organisation.md`: "It answers the visitor's chat messages as a helpful general assistant."
- **Components:** _no linked components_

### Rule 7

Replies must start within a few seconds.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "Replies start within a few seconds."
- **Components:** _no linked components_

### Rule 8

The conversation stays in the browser; there is no database and no sign-in.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "The conversation stays in the browser; there is no database and no sign-in."
- **Components:** _no linked components_

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

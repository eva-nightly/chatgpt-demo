# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

Harmless requests must not be refused; unsafe requests are declined politely.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "A good answer is correct, relevant to the question, clearly written, and refuses nothing harmless."
  - `business.md`: "Harmless requests are not refused; unsafe ones are declined politely."
- **Components:** _no linked components_

### Rule 2

Answers must be correct, relevant to the question, and clearly written.

- **Verifiable:** ❌ no
- **Sources:**
  - `About_the_organisation.md`: "A good answer is correct, relevant to the question, clearly written, and refuses nothing harmless."
  - `business.md`: "Answers are correct, relevant and clearly written."
- **Components:** _no linked components_

### Rule 3

Conversations are kept in the browser only; there must be no database and no sign-in.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "Conversations are kept in the browser only; there is no database and no sign-in."
- **Components:** _no linked components_

### Rule 4

Replies must start streaming within a couple of seconds.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "Replies start streaming within a couple of seconds."
- **Components:** _no linked components_

### Rule 5

Errors (e.g. bad key, rate limit) must be explained in plain language; never show a blank screen.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "Errors (bad key, rate limit) are explained in plain language, never a blank screen."
- **Components:** _no linked components_

### Rule 6

The AI must be reached via OpenRouter using an OpenAI-compatible API, with the base URL set by OPENAI_API_BASE_URL.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "The AI is reached through OpenRouter using an OpenAI-compatible API (base URL set by OPENAI_API_BASE_URL)."
- **Components:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 10 · rule: 0/6 · usp: 0/4
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (10)

- **usp** Minimal single-page streaming chat: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** OpenRouter / OpenAI-compatible backend: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Self-hosted and private by design: The only words that matched a name, path or route are too short to mean one thing (page), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Open source, small codebase: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** Harmless requests must not be refused; unsafe requests are declined politely.: No artifact mentions any of: answ, clearly, correct, declin, good, harmles, politely, question, refus, relevant, request, unsafe, writt.
- **rule** Answers must be correct, relevant to the question, and clearly written.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** Conversations are kept in the browser only; there must be no database and no sign-in.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Replies must start streaming within a couple of seconds.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Errors (e.g. bad key, rate limit) must be explained in plain language; never show a blank screen.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** The AI must be reached via OpenRouter using an OpenAI-compatible API, with the base URL set by OPENAI_API_BASE_URL.: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.

## Gaps

_None. All material was sourced._

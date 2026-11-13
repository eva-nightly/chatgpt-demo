# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

Answers must be correct, relevant and clearly written.

- **Verifiable:** ❌ no
- **Sources:**
  - `About_the_organisation.md`: "A good answer is correct, relevant, clearly written, and respects the system prompt and conversation history."
  - `about-chatgpt-demo.md`: "Answers are correct, relevant and clearly written."
- **Components:** _no linked components_

### Rule 2

The assistant must follow the system prompt and respect the conversation history (remember earlier turns).

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "A good answer is correct, relevant, clearly written, and respects the system prompt and conversation history."
  - `about-chatgpt-demo.md`: "The assistant follows the system prompt and remembers earlier turns."
- **Components:** _no linked components_

### Rule 3

Errors from the AI provider must be shown in plain language, never as raw stack traces.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "Errors from the AI provider are shown in plain language, never as raw stack traces."
- **Components:** _no linked components_

### Rule 4

Replies must start streaming within a couple of seconds.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "Replies start streaming within a couple of seconds."
- **Components:** _no linked components_

### Rule 5

Conversation history is kept in the browser; there is no database.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "The conversation history is kept in the browser; there is no database."
- **Components:** _no linked components_

### Rule 6

The AI is reached through an OpenAI-compatible API, configured by OPENAI_API_BASE_URL.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "The AI is reached through an OpenAI-compatible API (OpenRouter), set by OPENAI_API_BASE_URL."
- **Components:** _no linked components_

### Rule 7

Users can chat without signing in.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about-chatgpt-demo.md`: "It is aimed at individual people and small teams who want a fast, no-frills chat without sign-in."
- **Components:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 13 · rule: 0/7 · usp: 0/6
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (13)

- **usp** Minimal, fast web chat with an AI assistant: The only words that matched a name, path or route are too short to mean one thing (api, open, type), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Streaming replies: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** OpenAI-compatible API backend: The only words that matched a name, path or route are too short to mean one thing (open, type), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** No sign-in required: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **usp** Conversation history kept in the browser: No artifact mentions any of: behind, brows, conversation, database, history, kept, live, product.
- **usp** Configurable system prompt: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Answers must be correct, relevant and clearly written.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** The assistant must follow the system prompt and respect the conversation history (remember earlier turns).: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Errors from the AI provider must be shown in plain language, never as raw stack traces.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Replies must start streaming within a couple of seconds.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Conversation history is kept in the browser; there is no database.: No artifact mentions any of: brows, conversation, database, history, kept.
- **rule** The AI is reached through an OpenAI-compatible API, configured by OPENAI_API_BASE_URL.: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** Users can chat without signing in.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.

## Gaps

_None. All material was sourced._

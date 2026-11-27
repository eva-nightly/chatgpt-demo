# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

The assistant should stream an answer after the user types a message.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "A minimal chat assistant: the user types a question and gets a helpful, correct, on-topic answer streamed back."
  - `business.md`: "The user types a message and the assistant streams back an answer."
- **Components:** _no linked components_

### Rule 2

The conversation should keep context across turns.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "Right means the answer is accurate, answers what was asked, and the chat keeps context across turns."
  - `business.md`: "The conversation keeps context across turns."
- **Components:** _no linked components_

### Rule 3

Answers should be accurate, on-topic, and concise.

- **Verifiable:** ❌ no
- **Sources:**
  - `About_the_organisation.md`: "Right means the answer is accurate, answers what was asked, and the chat keeps context across turns."
  - `business.md`: "Answers are accurate, on-topic and concise."
- **Components:** _no linked components_

### Rule 4

The chat should not leak the system prompt.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "The chat does not leak the system prompt, does not crash on long input, and handles errors from the model provider gracefully."
- **Components:** _no linked components_

### Rule 5

The chat should not crash on long input.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "The chat does not leak the system prompt, does not crash on long input, and handles errors from the model provider gracefully."
- **Components:** _no linked components_

### Rule 6

The chat should handle model-provider errors gracefully.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "The chat does not leak the system prompt, does not crash on long input, and handles errors from the model provider gracefully."
- **Components:** _no linked components_

### Rule 7

The AI should be reached through OpenRouter via the OPENAI_API_BASE_URL setting.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "The AI is reached through OpenRouter, via the OPENAI_API_BASE_URL setting."
- **Components:** _no linked components_

### Rule 8

The product has no sign-in and no database.

- **Verifiable:** ✅ yes
- **Sources:**
  - `business.md`: "There is no sign-in and no database."
- **Components:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 12 · rule: 0/8 · usp: 0/4
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (12)

- **usp** Minimal web chat interface: The only words that matched a name, path or route are too short to mean one thing (api), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Streaming answers: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Conversation context across turns: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** OpenAI-compatible API support: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** The assistant should stream an answer after the user types a message.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** The conversation should keep context across turns.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Answers should be accurate, on-topic, and concise.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** The chat should not leak the system prompt.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** The chat should not crash on long input.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** The chat should handle model-provider errors gracefully.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** The AI should be reached through OpenRouter via the OPENAI_API_BASE_URL setting.: The only words that matched a name, path or route are too short to mean one thing (open), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** The product has no sign-in and no database.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.

## Gaps

_None. All material was sourced._

# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Minimal web chat interface

A minimal web interface for chatting with ChatGPT or a large language model.

- **Sources:**
  - `About_the_organisation.md`: "Minimal web UI for ChatGPT."
  - `business.md`: "ChatGPT-API Demo is a minimal web chat interface for talking to a large language model."
- **Delivered by:** _no linked components_

## Streaming answers

The user types a message and the assistant streams back an answer.

- **Sources:**
  - `About_the_organisation.md`: "A minimal chat assistant: the user types a question and gets a helpful, correct, on-topic answer streamed back."
  - `business.md`: "The user types a message and the assistant streams back an answer."
- **Delivered by:** _no linked components_

## Conversation context across turns

The conversation keeps context across turns.

- **Sources:**
  - `About_the_organisation.md`: "A minimal chat assistant: the user types a question and gets a helpful, correct, on-topic answer streamed back."
  - `business.md`: "The conversation keeps context across turns."
- **Delivered by:** _no linked components_

## OpenAI-compatible API support

The chat reaches the AI through OpenRouter using the OPENAI_API_BASE_URL setting.

- **Sources:**
  - `business.md`: "Developers and hobbyists who want a lightweight, self-hosted chat UI on top of an OpenAI-compatible API."
  - `business.md`: "The AI is reached through OpenRouter, via the OPENAI_API_BASE_URL setting."
- **Delivered by:** _no linked components_

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

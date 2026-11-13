# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Minimal, fast web chat with an AI assistant

A no-frills web chat UI where people type messages and get answers from an AI model, built for a simple, fast experience.

- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat UI where people type messages and get answers from an AI model through an OpenAI-compatible API."
  - `About_the_organisation.md`: "Just me, for now; I am building it for people who want a simple, fast chat with an AI assistant."
  - `about-chatgpt-demo.md`: "ChatGPT-API Demo is a minimal web chat interface for talking to an AI model."
  - `about-chatgpt-demo.md`: "It is aimed at individual people and small teams who want a fast, no-frills chat without sign-in."
- **Delivered by:** _no linked components_

## Streaming replies

The AI's answer streams in as it is generated rather than arriving all at once.

- **Sources:**
  - `About_the_organisation.md`: "It answers the user's questions in a chat, streaming the reply."
  - `about-chatgpt-demo.md`: "Users type a message and see the AI's answer stream in."
  - `about-chatgpt-demo.md`: "Replies start streaming within a couple of seconds."
- **Delivered by:** _no linked components_

## OpenAI-compatible API backend

The AI is reached through an OpenAI-compatible API (OpenRouter), configured via OPENAI_API_BASE_URL.

- **Sources:**
  - `About_the_organisation.md`: "A minimal web chat UI where people type messages and get answers from an AI model through an OpenAI-compatible API."
  - `about-chatgpt-demo.md`: "The AI is reached through an OpenAI-compatible API (OpenRouter), set by OPENAI_API_BASE_URL."
- **Delivered by:** _no linked components_

## No sign-in required

Individuals and small teams can start chatting without creating an account or signing in.

- **Sources:**
  - `about-chatgpt-demo.md`: "It is aimed at individual people and small teams who want a fast, no-frills chat without sign-in."
- **Delivered by:** _no linked components_

## Conversation history kept in the browser

History lives in the browser; there is no database behind the product.

- **Sources:**
  - `about-chatgpt-demo.md`: "The conversation history is kept in the browser; there is no database."
- **Delivered by:** _no linked components_

## Configurable system prompt

A system prompt can be set to steer the assistant's behaviour.

- **Sources:**
  - `about-chatgpt-demo.md`: "A system prompt can be set to steer the assistant's behaviour."
- **Delivered by:** _no linked components_

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

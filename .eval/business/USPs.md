# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Minimal AI chat page

A minimal web chat page for talking to an AI assistant.

- **Sources:**
  - `About_the_organisation.md`: "Minimal web UI for ChatGPT."
  - `business.md`: "ChatGPT-API Demo is a minimal web chat page that lets a person talk to an AI assistant."
- **Delivered by:** _no linked components_

## Streaming responses

Answers stream back into the page like a normal chat.

- **Sources:**
  - `business.md`: "The visitor types a message and the page sends the conversation to an OpenAI-compatible API (through OpenRouter)."
  - `business.md`: "The answer streams back into the page, like a normal chat."
- **Delivered by:** _no linked components_

## Ongoing conversations

Visitors can continue a conversation over several turns and clear it.

- **Sources:**
  - `business.md`: "Visitors can keep a conversation going over several turns, and can clear it."
- **Delivered by:** _no linked components_

## No sign-in or server-side storage

Visitors do not need to sign in, and nothing is stored on a server.

- **Sources:**
  - `business.md`: "There is no sign-in and no database: nothing is stored on a server."
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 11 · rule: 0/7 · usp: 0/4
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (11)

- **usp** Minimal AI chat page: The only words that matched a name, path or route are too short to mean one thing (api, page), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Streaming responses: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Ongoing conversations: 1 candidate(s) were offered and the model confirmed none of them.
- **usp** No sign-in or server-side storage: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Answers should be helpful, accurate, on topic, and in the visitor's language.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** Send the visitor's message and conversation to an OpenAI-compatible API through OpenRouter.: The only words that matched a name, path or route are too short to mean one thing (api, open, page, type), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** Stream the answer back into the page.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Allow visitors to continue a conversation over several turns and clear it.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** Do not require sign-in or store visitor data on a server.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Answers should arrive quickly and should not be cut off or replaced by raw error text.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** When the AI service fails, explain the failure plainly and let the visitor try again.: No artifact mentions any of: explain, fail, failure, let, plainly, service, try, visitor.

## Gaps

_None. All material was sourced._

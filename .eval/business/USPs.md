# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Streamed answers from an LLM in a minimal chat page

A visitor types a message and receives a streamed answer from an OpenAI-compatible model via OpenRouter; answers arrive quickly and the page stays responsive.

- **Sources:**
  - `About_the_organisation.md`: "A minimal chat web UI: the user types a message and gets a streamed answer from an OpenAI-compatible model through OpenRouter."
  - `product.md`: "A visitor types a question and receives an answer from a large language model."
  - `product.md`: "Answers stream in quickly; the page stays responsive."
- **Delivered by:** _no linked components_

## Simple and private, with no accounts

Designed as a simple private chat UI for people who want no sign-in, no database and no payments.

- **Sources:**
  - `About_the_organisation.md`: "Just me, for now; I am building it as a demo for people who want a simple private chat page."
  - `product.md`: "Individual developers and curious people who want a simple, private chat UI without accounts."
  - `product.md`: "No sign-in, no database, no payments."
- **Delivered by:** _no linked components_

## Conversation context is kept across turns

The chat keeps its conversation context so follow-up questions build on earlier turns.

- **Sources:**
  - `About_the_organisation.md`: "Answers the user's question in a clear, correct, concise way, keeps conversation context, and shows a helpful error when the model fails."
  - `product.md`: "The conversation keeps its context across turns."
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 0 of 9 · rule: 0/6 · usp: 0/3
- **Artifacts reached from the business:** 0 of 35 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Other: 0 of 18
- Utils: 0 of 7
- Icons: 0 of 4
- Pages: 0 of 4
- Plugins: 0 of 2

### Linked to nothing (9)

- **usp** Streamed answers from an LLM in a minimal chat page: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** Simple and private, with no accounts: The only words that matched a name, path or route are too short to mean one thing (page), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Conversation context is kept across turns: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** Answers must be relevant, correct and concise.: This rule says of itself that no machine can check it, so no code implements it and anything the words matched would be a coincidence. Mark it verifiable to have it searched for.
- **rule** The conversation keeps its context across turns.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** When the model service fails or the API key is wrong, the user sees a clear, polite error.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** The model is reached through an OpenAI-compatible API (OpenRouter), configured by OPENAI_API_BASE_URL.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Answers stream in quickly and the page stays responsive.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** No sign-in, no database, no payments.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.

## Gaps

_None. All material was sourced._

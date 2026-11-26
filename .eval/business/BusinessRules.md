# Business rules

_Each rule is sourced verbatim, marked verifiable (yes/no), and linked to the components it governs._

### Rule 1

Replies must be in the language the visitor wrote in.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "Right means a clear, correct, relevant reply to what they asked, in the language they wrote in, without making things up."
  - `about.md`: "Answers are correct, relevant, and in the language the visitor wrote in."
- **Components:** _no linked components_

### Rule 2

The assistant must admit when it does not know instead of inventing facts; wrong or invented answers presented confidently are unacceptable.

- **Verifiable:** ✅ yes
- **Sources:**
  - `About_the_organisation.md`: "Right means a clear, correct, relevant reply to what they asked, in the language they wrote in, without making things up."
  - `about.md`: "The assistant admits when it does not know instead of inventing facts."
  - `about.md`: "Wrong or invented answers presented confidently."
- **Components:** _no linked components_

### Rule 3

Replies must stream quickly and must not cut off mid-sentence.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "Replies stream quickly and do not cut off mid-sentence."
- **Components:** _no linked components_

### Rule 4

Replies must not ignore a system instruction set by the owner.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "Replies ignoring a system instruction set by the owner."
- **Components:** _no linked components_

### Rule 5

Errors must not be shown to the visitor when the model provider is slow or unavailable.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "Errors shown to the visitor when the model provider is slow or unavailable."
- **Components:** _no linked components_

### Rule 6

Long conversations must keep context and stay coherent.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "Long conversations keep context and stay coherent."
- **Components:** _no linked components_

### Rule 7

There is no sign-in and no database; conversations live only in the browser.

- **Verifiable:** ✅ yes
- **Sources:**
  - `about.md`: "There is no sign-in and no database; conversations live in the browser."
- **Components:** _no linked components_

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

- **usp** Minimal web chat UI: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **usp** General assistant behaviour: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **usp** No accounts, no database: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **usp** Streamed answers: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Replies must be in the language the visitor wrote in.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** The assistant must admit when it does not know instead of inventing facts; wrong or invented answers presented confidently are unacceptable.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** Replies must stream quickly and must not cut off mid-sentence.: Everything that matched is shared plumbing rather than something a business statement can be about: parseOpenAIStream (it is a "parse" helper: it changes the shape of a value and decides nothing).
- **rule** Replies must not ignore a system instruction set by the owner.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Errors must not be shown to the visitor when the model provider is slow or unavailable.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** Long conversations must keep context and stay coherent.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.
- **rule** There is no sign-in and no database; conversations live only in the browser.: No artifact NAME, path, route or endpoint in the codebase matches any word in it. It may be a rule about how people work rather than about what the product does.

## Gaps

_None. All material was sourced._

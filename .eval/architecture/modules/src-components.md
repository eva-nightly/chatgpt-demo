# Module: src/components

Provides the Solid.js UI component layer for the chat application, managing message history, streaming LLM completions from the backend API, configuring system prompts and temperature, and rendering markdown-formatted conversation history.

## Key files
- `src/components/Generator.tsx`: Main chat orchestrator component managing message list state, streaming POST requests to /api/generate, scroll positioning, and conversation persistence.
- `src/components/MessageItem.tsx`: Renders individual chat messages with markdown parsing, KaTeX math rendering, code highlighting, and copy-to-clipboard functionality.
- `src/components/SystemRoleSettings.tsx`: Panel for setting system role instructions and tuning model temperature prior to starting conversations.
- `src/components/ErrorMessageItem.tsx`: Displays formatted error messages from API calls with a retry action.
- `src/components/Slider.tsx`: Zag.js-powered slider component used for numerical settings like temperature.
- `src/components/SettingsSlider.tsx`: Wrapper component binding setting configurations to the Slider.
- `src/components/icons/Clear.tsx`: SVG icon for clearing chat history.
- `src/components/icons/Env.tsx`: SVG icon representing environment/system settings.
- `src/components/icons/Refresh.tsx`: SVG icon representing retry/regenerate action.
- `src/components/icons/X.tsx`: SVG icon for cancel/delete actions.

## Public interface
- default (src/components/Generator.tsx)
- default (src/components/MessageItem.tsx)
- default (src/components/SystemRoleSettings.tsx)
- default (src/components/ErrorMessageItem.tsx)
- Slider (src/components/Slider.tsx)
- default (src/components/SettingsSlider.tsx)
- default (src/components/icons/Clear.tsx)
- default (src/components/icons/Env.tsx)
- default (src/components/icons/Refresh.tsx)
- default (src/components/icons/X.tsx)

## Dependencies
- solid-js
- solidjs-use
- @zag-js/slider
- @zag-js/solid
- markdown-it
- markdown-it-katex
- markdown-it-highlightjs
- @/utils/auth
- @/types
- @/types/provider
- ../slider.css

## AI touchpoints [AI]
- `src/components/Generator.tsx`
- `src/components/SystemRoleSettings.tsx`

## Where the code disagrees with the stack profile
- `src/components/Generator.tsx`: The UI is built using Solid.js reactive primitives and Vite/Astro-style env variables (`import.meta.env.PUBLIC_MAX_HISTORY_MESSAGES`) rather than Next.js React components and `process.env`.

## Open questions
- How does the client recover if a stream connection abruptly drops mid-generation without a clean EOF?

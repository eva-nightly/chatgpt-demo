# Module: src/components

Provides the SolidJS frontend UI components for the web chat interface, handling client-side conversation state, message rendering with Markdown/LaTeX, system prompt configuration, temperature adjustment, and streaming AI response orchestration.

## Key files
- `src/components/Generator.tsx`: Main chat generator controller managing message lists, session storage persistence, streaming fetch calls to /api/generate, scrolling, and error handling.
- `src/components/MessageItem.tsx`: Renders formatted markdown chat turns (user/assistant/system) with code block syntax highlighting, KaTeX math parsing, copy buttons, and retry actions.
- `src/components/SystemRoleSettings.tsx`: Interface for defining the assistant system prompt and configuring generation temperature before starting a chat.
- `src/components/ErrorMessageItem.tsx`: Displays user-facing error messages from the API with code details and a regeneration button.
- `src/components/Slider.tsx`: Zag.js-powered accessible slider component for adjusting numeric parameters like temperature.
- `src/components/SettingsSlider.tsx`: Wrapper component mapping provider slider settings schemas to the Slider UI component.

## Public interface
- default export (Generator) from src/components/Generator.tsx
- default export (MessageItem) from src/components/MessageItem.tsx
- default export (SystemRoleSettings) from src/components/SystemRoleSettings.tsx
- default export (ErrorMessageItem) from src/components/ErrorMessageItem.tsx
- default export (SettingsSlider) from src/components/SettingsSlider.tsx
- Slider export from src/components/Slider.tsx
- default export (Clear icon) from src/components/icons/Clear.tsx
- default export (Env icon) from src/components/icons/Env.tsx
- default export (Refresh icon) from src/components/icons/Refresh.tsx
- default export (X icon) from src/components/icons/X.tsx

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

## AI touchpoints [AI]
- `src/components/Generator.tsx`
- `src/components/SystemRoleSettings.tsx`

## Where the code disagrees with the stack profile
- `src/components/Generator.tsx`: The codebase uses SolidJS and client-side Vite/Astro environment variables (import.meta.env.PUBLIC_MAX_HISTORY_MESSAGES) rather than standard Next.js React and process.env runtime conventions.

## Open questions
- _none_

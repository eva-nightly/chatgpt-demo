# Module: src/components

Provides the frontend UI components built with Solid.js for ChatGPT-API Demo, including the interactive chat interface, streaming response reader, markdown/code rendering, system prompt configuration, error displays, and temperature controls.

## Key files
- `src/components/Generator.tsx`: Main chat interface component managing message history, streaming fetch requests to /api/generate, session storage persistence, scroll management, and user input.
- `src/components/MessageItem.tsx`: Renders chat messages with Markdown, KaTeX math formatting, syntax-highlighted code blocks with copy-to-clipboard buttons, and retry controls.
- `src/components/SystemRoleSettings.tsx`: Interface for configuring custom system role prompt instructions and temperature parameters.
- `src/components/ErrorMessageItem.tsx`: Displays formatted error messages, error codes, and a regenerate retry button when API requests fail.
- `src/components/Slider.tsx`: State machine slider input built using Zag.js to adjust numerical settings like temperature.
- `src/components/SettingsSlider.tsx`: Adapter component wrapping Slider for generic UI settings configurations.

## Public interface
- default (from src/components/Generator.tsx)
- default (from src/components/MessageItem.tsx)
- default (from src/components/SystemRoleSettings.tsx)
- default (from src/components/ErrorMessageItem.tsx)
- default (from src/components/SettingsSlider.tsx)
- Slider (from src/components/Slider.tsx)
- default (from src/components/icons/Clear.tsx)
- default (from src/components/icons/Env.tsx)
- default (from src/components/icons/Refresh.tsx)
- default (from src/components/icons/X.tsx)

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
- `src/components/Generator.tsx`: Components are built with Solid.js and use Vite/Astro-style import.meta.env rather than React and Next.js.

## Open questions
- _none_

# Module: src/components

Provides SolidJS UI components for rendering the chat interface, managing chat streams, editing system role instructions and temperature settings, displaying markdown-formatted and KaTeX-rendered messages, and handling error states.

## Key files
- `src/components/Generator.tsx`: Main chat container managing message state, sessionStorage/localStorage synchronization, stream fetching, abort controller, and scroll handling.
- `src/components/MessageItem.tsx`: Renders individual chat messages with Markdown, KaTeX, highlight.js syntax highlighting, code snippet copying, and retry triggers.
- `src/components/SystemRoleSettings.tsx`: UI for editing assistant system role prompts and setting temperature via a slider.
- `src/components/ErrorMessageItem.tsx`: Renders formatted API error alerts with an optional retry/regeneration button.
- `src/components/SettingsSlider.tsx`: Wrapper around the slider component for dynamic settings configuration.
- `src/components/Slider.tsx`: Accessible slider component powered by @zag-js/slider for numeric inputs like temperature.
- `src/components/icons/Clear.tsx`: SVG clear icon component.
- `src/components/icons/Env.tsx`: SVG environment/settings icon component.
- `src/components/icons/Refresh.tsx`: SVG refresh/regenerate icon component.
- `src/components/icons/X.tsx`: SVG close/dismiss icon component.

## Public interface
- default (src/components/Generator.tsx)
- default (src/components/MessageItem.tsx)
- default (src/components/ErrorMessageItem.tsx)
- default (src/components/SystemRoleSettings.tsx)
- default (src/components/SettingsSlider.tsx)
- Slider (src/components/Slider.tsx)
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
- @/types
- @/types/provider
- @/utils/auth

## AI touchpoints [AI]
- `src/components/Generator.tsx`
- `src/components/SystemRoleSettings.tsx`

## Where the code disagrees with the stack profile
- `src/components/Generator.tsx`: The UI is built with SolidJS and Vite/Astro client-side conventions (import.meta.env.PUBLIC_MAX_HISTORY_MESSAGES, solid-js imports) rather than Next.js React components.

## Open questions
- The trailing part of src/components/Generator.tsx is truncated in the source snippet.

# Module: (root) [AI]

Provides root-level build, linting, type-checking, styling, and framework configuration for ChatGPT-API Demo using Astro, SolidJS, and UnoCSS with multi-platform deployment adapters (Node, Vercel, Netlify).

## Key files
- `astro.config.mjs`: Configures Astro build and server settings, SolidJS and UnoCSS integrations, PWA manifest and service worker options, deployment adapters (Node standalone, Vercel Edge, Netlify Edge Functions), and Vite plugins.
- `unocss.config.ts`: Defines UnoCSS styling presets, typography extensions, and design utility shortcuts used across the chat user interface components.
- `.eslintrc.js`: Configures ESLint rules and parsing overrides for JavaScript, TypeScript, and Astro templates.
- `shims.d.ts`: Provides TypeScript declarations augmenting JSX and astroHTML interfaces for UnoCSS attributify support.

## Public interface
- export default defineConfig(...) (astro.config.mjs)
- export default defineConfig(...) (unocss.config.ts)
- module.exports (eslintrc.js)

## Dependencies
- astro/config
- unocss/astro
- @astrojs/solid-js
- @astrojs/node
- @vite-pwa/astro
- @astrojs/vercel/edge
- @astrojs/netlify/edge-functions
- ./plugins/disableBlocks
- unocss
- @unocss/preset-attributify

## AI touchpoints [AI]
- `astro.config.mjs`

## Where the code disagrees with the stack profile
- `astro.config.mjs`: The repository uses Astro with SolidJS and configurable server adapters (Node.js standalone, Vercel Edge, Netlify Edge Functions), not Next.js or Next route handlers.

## Open questions
- _none_

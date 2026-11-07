# Module: (root) [AI]

Provides root-level build, deployment, styling, type declaration, and linting configurations for the Astro-based ChatGPT-API Demo application.

## Key files
- `astro.config.mjs`: Configures Astro SSR output, integrations (Solid.js, UnoCSS, PWA), Vite plugins, and deployment adapters (Node standalone, Vercel Edge, Netlify Edge Functions).
- `unocss.config.ts`: Configures UnoCSS atomic styling presets, typography, icon CDN, transformers, and UI shortcut classes for chat components.
- `.eslintrc.js`: Defines ESLint configuration and parsing overrides for Astro and TypeScript components.
- `shims.d.ts`: Extends global JSX and HTML attribute definitions with UnoCSS Attributify typings.

## Public interface
- astro.config.mjs (default export Astro configuration)
- unocss.config.ts (default export UnoCSS configuration)
- .eslintrc.js (module.exports ESLint configuration)

## Dependencies
- astro
- @astrojs/solid-js
- @astrojs/node
- @astrojs/vercel
- @astrojs/netlify
- @vite-pwa/astro
- unocss
- @unocss/preset-attributify
- @unocss/preset-icons
- @unocss/preset-typography
- @unocss/preset-uno
- @evan-yang
- plugin:astro/recommended
- astro-eslint-parser
- @typescript-eslint/parser

## AI touchpoints [AI]
- `astro.config.mjs`

## Where the code disagrees with the stack profile
- `astro.config.mjs`: The stack describes the repository as a Next.js application using Next route handlers, but the project is configured as an Astro application using Solid.js and configurable deployment adapters (Node, Vercel Edge, Netlify Edge).

## Open questions
- _none_

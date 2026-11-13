# Module: (root) [AI]

Root configuration and environment setup for ChatGPT-API Demo, defining the Astro build/deployment adapter integration, PWA generation, UnoCSS styling rules, TypeScript JSX shims, and ESLint linting rules.

## Key files
- `astro.config.mjs`: Configures the Astro application build pipeline, including integrations (UnoCSS, Solid.js, AstroPWA) and runtime adapter selection (Vercel Edge, Netlify Edge, or Node standalone).
- `unocss.config.ts`: Defines UnoCSS styling presets, typography configurations, and custom utility shortcut classes for chat interface elements.
- `.eslintrc.js`: Sets linting configurations and parsing rules for TypeScript and Astro templates.
- `shims.d.ts`: Provides ambient TypeScript type declarations for UnoCSS JSX attributify attributes in Astro and generic JSX templates.

## Public interface
- default export in astro.config.mjs (Astro configuration object)
- default export in unocss.config.ts (UnoCSS configuration object)
- module.exports in .eslintrc.js (ESLint configuration object)

## Dependencies
- @astrojs/netlify/edge-functions
- @astrojs/node
- @astrojs/solid-js
- @astrojs/vercel/edge
- @evan-yang
- @typescript-eslint/parser
- @unocss/preset-attributify
- @vite-pwa/astro
- astro/config
- astro-eslint-parser
- plugin:astro/recommended
- unocss
- unocss/astro
- ./plugins/disableBlocks

## AI touchpoints [AI]
- `astro.config.mjs`

## Where the code disagrees with the stack profile
- `astro.config.mjs`: The scan indicated Next route handlers with Next.js API routes in src/pages/api/, but the repository actually uses Astro (`astro.config.mjs`) configured with Solid.js (`@astrojs/solid-js`) and multi-adapter deployment support (Node, Vercel Edge, Netlify Edge).

## Open questions
- _none_

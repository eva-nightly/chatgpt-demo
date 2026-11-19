# Module: (root) [AI]

Root configuration and environment definitions for the application, configuring Astro server-side rendering adapters, UnoCSS styling shortcuts, PWA capabilities, TypeScript JSX shims, and ESLint rules.

## Key files
- `astro.config.mjs`: Defines Astro project configuration, integrations (UnoCSS, SolidJS, PWA), server adapters (Node, Vercel Edge, Netlify Edge), and Vite plugins.
- `unocss.config.ts`: Defines UnoCSS utility presets, transformers, and custom design system shortcuts tailored for the chat UI.
- `.eslintrc.js`: Configures linting rules and parsers for JavaScript, TypeScript, and Astro single-file components.
- `shims.d.ts`: Declares global TypeScript ambient namespaces to support UnoCSS attributify JSX attributes across Astro and Solid components.

## Public interface
- Default export from astro.config.mjs (Astro configuration object)
- Default export from unocss.config.ts (UnoCSS configuration object)
- module.exports from .eslintrc.js (ESLint configuration object)

## Dependencies
- astro/config
- unocss/astro
- @astrojs/solid-js
- @astrojs/node
- @vite-pwa/astro
- @astrojs/vercel/edge
- @astrojs/netlify/edge-functions
- unocss
- @unocss/preset-attributify

## AI touchpoints [AI]
- `astro.config.mjs`

## Where the code disagrees with the stack profile
- `astro.config.mjs`: The project uses Astro with SolidJS and SSR adapters (Node, Vercel Edge, Netlify Edge) rather than Next.js route handlers.

## Open questions
- _none_

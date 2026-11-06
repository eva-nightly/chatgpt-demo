# Module: (root) [AI]

Provides root-level build, linting, type augmentation, and styling configurations for an Astro SSR project with SolidJS, UnoCSS, and PWA capabilities.

## Key files
- `astro.config.mjs`: Configures Astro SSR deployment adapters (Node, Vercel, Netlify), integrations (UnoCSS, SolidJS, Vite PWA), and Vite plugins
- `unocss.config.ts`: Configures UnoCSS presets, typography, icons, attribute mode, and custom UI style shortcut classes
- `.eslintrc.js`: Configures ESLint rules and TypeScript/Astro parser overrides
- `shims.d.ts`: Augments global JSX and Astro JSX namespaces with UnoCSS attributify types

## Public interface
- astro.config.mjs (default Astro configuration export)
- unocss.config.ts (default UnoCSS configuration export)
- .eslintrc.js (CommonJS ESLint configuration export)

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
- ./plugins/disableBlocks

## AI touchpoints [AI]
- `astro.config.mjs`

## Where the code disagrees with the stack profile
- `astro.config.mjs`: The repository is configured as an Astro application using SolidJS and Astro SSR adapters (Node, Vercel Edge, Netlify Edge) instead of Next.js route handlers.

## Open questions
- _none_

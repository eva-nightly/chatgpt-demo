# Module: plugins

Provides a build plugin (named 'vercel-disable-blocks') that strips delimited code blocks marked between '#vercel-disable-blocks' and '#vercel-end' in the generation API route ('pages/api/generate.ts').

## Key files
- `plugins/disableBlocks.ts`: Vite/Rollup-compatible build plugin that strips marked code blocks from 'pages/api/generate.ts' during pre-enforcement transformation.

## Public interface
- default plugin()

## Dependencies
- _none_

## Open questions
- _none_

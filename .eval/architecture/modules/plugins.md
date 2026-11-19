# Module: plugins

Provides a build plugin (named 'vercel-disable-blocks') that strips out code sections demarcated by '#vercel-disable-blocks' and '#vercel-end' inside 'pages/api/generate.ts' during build transformations.

## Key files
- `plugins/disableBlocks.ts`: Defines and exports a pre-enforced build plugin that strips specified comment-blocked code in pages/api/generate.ts.

## Public interface
- export default function plugin(): { name: string; enforce: string; transform: (code: string, id: string) => { code: string; map: null } | undefined }

## Dependencies
- _none_

## Open questions
- _none_

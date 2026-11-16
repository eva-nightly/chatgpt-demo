# Module: plugins

Provides a build plugin that strips designated code sections bounded by '#vercel-disable-blocks' and '#vercel-end' markers from the API route file 'pages/api/generate.ts'.

## Key files
- `plugins/disableBlocks.ts`: Implements the 'vercel-disable-blocks' transform plugin configured with pre-enforcement to strip specific comment blocks from pages/api/generate.ts.

## Public interface
- export default function plugin(): { name: string, enforce: 'pre', transform: (code: string, id: string) => { code: string, map: null } | undefined }

## Dependencies
- _none_

## Open questions
- _none_

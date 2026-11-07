# Module: plugins

Provides a build plugin (named vercel-disable-blocks) to strip designated code sections enclosed by #vercel-disable-blocks and #vercel-end comment markers in pages/api/generate.ts prior to compilation.

## Key files
- `plugins/disableBlocks.ts`: Exports a build-time pre-transform plugin that removes marked code blocks from pages/api/generate.ts.

## Public interface
- export default function plugin(): { name: string, enforce: 'pre', transform: (code: string, id: string) => { code: string, map: null } | undefined }

## Dependencies
- _none_

## AI touchpoints [AI]
- `plugins/disableBlocks.ts`

## Open questions
- _none_

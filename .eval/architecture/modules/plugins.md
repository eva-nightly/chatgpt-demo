# Module: plugins

Provides a build plugin to strip out designated code blocks marked with #vercel-disable-blocks in pages/api/generate.ts during compilation or bundling.

## Key files
- `plugins/disableBlocks.ts`: Defines a build plugin that removes code sections between #vercel-disable-blocks and #vercel-end tags in the generate API route file.

## Public interface
- default function plugin(): { name: string, enforce: string, transform: (code: string, id: string) => { code: string, map: null } | undefined }

## Dependencies
- _none_

## Open questions
- _none_

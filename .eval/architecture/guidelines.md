# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Use Astro/Vite's import.meta.env for runtime configuration in endpoints and utilities.

- `src/pages/api/auth.ts`:

  ```
  const realPassword = import.meta.env.SITE_PASSWORD || ''
  ```

- `src/pages/api/generate.ts`:

  ```
  const apiKey = import.meta.env.OPENAI_API_KEY
  ```

- `src/pages/api/generate.ts`:

  ```
  const httpsProxy = import.meta.env.HTTPS_PROXY
  ```

- `src/utils/openAI.ts`:

  ```
  export const model = import.meta.env.OPENAI_API_MODEL || 'gpt-3.5-turbo'
  ```

## Keep environment variable typings in the ImportMetaEnv and ImportMeta interfaces.

- `src/env.d.ts`:

  ```
  interface ImportMetaEnv {
  ```

- `src/env.d.ts`:

  ```
  interface ImportMeta {
  ```

## Define component prop shapes with a Props interface and use that type in the component signature.

- `src/components/ErrorMessageItem.tsx`:

  ```
  interface Props {
  ```

- `src/components/ErrorMessageItem.tsx`:

  ```
  export default ({ data, onRetry }: Props) => {
  ```

- `src/components/MessageItem.tsx`:

  ```
  interface Props {
  ```

- `src/components/MessageItem.tsx`:

  ```
  export default ({ role, message, showRetry, onRetry }: Props) => {
  ```

- `src/components/SystemRoleSettings.tsx`:

  ```
  interface Props {
  ```

- `src/components/SystemRoleSettings.tsx`:

  ```
  export default (props: Props) => {
  ```

## Represent shared domain data shapes with exported TypeScript interfaces.

- `src/types.ts`:

  ```
  export interface ChatMessage {
  ```

- `src/types.ts`:

  ```
  export interface ErrorMessage {
  ```

## Export Astro and UnoCSS configuration through default defineConfig calls.

- `astro.config.mjs`:

  ```
  export default defineConfig({
  ```

- `unocss.config.ts`:

  ```
  export default defineConfig({
  ```

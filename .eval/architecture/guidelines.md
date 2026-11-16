# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Read configuration from import.meta.env (Astro/Vite style), providing a sensible default or empty fallback where appropriate; never use process.env.

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

## SolidJS components should be exported as default anonymous arrow functions that destructure or accept a locally declared `Props` interface.

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

## Declare a local `interface Props` directly above each component to type its inputs rather than using inline or shared prop types.

- `src/components/ErrorMessageItem.tsx`:

  ```
  interface Props {
  ```

- `src/components/MessageItem.tsx`:

  ```
  interface Props {
  ```

- `src/components/SettingsSlider.tsx`:

  ```
  interface Props {
  ```

- `src/components/Slider.tsx`:

  ```
  interface Props {
  ```

- `src/components/SystemRoleSettings.tsx`:

  ```
  interface Props {
  ```

## Icon components are stateless default-exported arrow functions with no props, kept in src/components/icons.

- `src/components/icons/Clear.tsx`:

  ```
  export default () => {
  ```

- `src/components/icons/Env.tsx`:

  ```
  export default () => {
  ```

- `src/components/icons/Refresh.tsx`:

  ```
  export default () => {
  ```

- `src/components/icons/X.tsx`:

  ```
  export default () => {
  ```

## Shared domain types live in src/types.ts as exported interfaces (e.g., ChatMessage, ErrorMessage) and are imported via the '@/types' alias.

- `src/types.ts`:

  ```
  export interface ChatMessage {
  ```

- `src/types.ts`:

  ```
  export interface ErrorMessage {
  ```

## Configuration files (Astro, UnoCSS) use the framework's `defineConfig` helper as a default export.

- `astro.config.mjs`:

  ```
  export default defineConfig({
  ```

- `unocss.config.ts`:

  ```
  export default defineConfig({
  ```

## Build-time and utility helpers are written as arrow or plain functions with explicit TypeScript parameter types, and exported as named consts when they are reusable utilities.

- `plugins/disableBlocks.ts`:

  ```
  const transform = (code: string, id: string) => {
  ```

- `src/utils/auth.ts`:

  ```
  async function digestMessage(message: string) {
  ```

- `src/utils/openAI.ts`:

  ```
  export const generatePayload = (
  ```

- `src/components/Slider.tsx`:

  ```
  export const Slider = (selectProps: Props) => {
  ```

## Ambient type declarations (env variables, JSX attribute augmentation) are placed in .d.ts files using interface merging rather than runtime code.

- `shims.d.ts`:

  ```
  interface HTMLAttributes extends AttributifyAttributes { }
  ```

- `shims.d.ts`:

  ```
  interface HTMLAttributes<> extends AttributifyAttributes {}
  ```

- `src/env.d.ts`:

  ```
  interface ImportMetaEnv {
  ```

- `src/env.d.ts`:

  ```
  interface ImportMeta {
  ```

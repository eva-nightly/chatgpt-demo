# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Declare a local `interface Props` at the top of each Solid.js component file to type its inputs, rather than inline prop types.

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

## Export components as anonymous default arrow functions; destructure or accept `Props` directly in the parameter list.

- `src/components/ErrorMessageItem.tsx`:

  ```
  export default ({ data, onRetry }: Props) => {
  ```

- `src/components/Generator.tsx`:

  ```
  export default () => {
  ```

- `src/components/MessageItem.tsx`:

  ```
  export default ({ role, message, showRetry, onRetry }: Props) => {
  ```

- `src/components/SystemRoleSettings.tsx`:

  ```
  export default (props: Props) => {
  ```

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

## Read configuration from `import.meta.env` (Astro/Vite convention), providing a sensible fallback with `||` where a value is optional.

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

## Use `export default defineConfig({...})` for tool configuration files (Astro, UnoCSS) to get typed config objects.

- `astro.config.mjs`:

  ```
  export default defineConfig({
  ```

- `unocss.config.ts`:

  ```
  export default defineConfig({
  ```

## Define shared data shapes as named exported TypeScript interfaces in dedicated type files; keep ambient env typings as non-exported `interface` augmentations.

- `src/types.ts`:

  ```
  export interface ChatMessage {
  ```

- `src/types.ts`:

  ```
  export interface ErrorMessage {
  ```

- `src/env.d.ts`:

  ```
  interface ImportMetaEnv {
  ```

- `src/env.d.ts`:

  ```
  interface ImportMeta {
  ```

## Keep non-component helpers (transforms, digest functions, payload builders) as standalone `const`/`function` definitions with explicit parameter types, exporting only what other modules need.

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

- `astro.config.mjs`:

  ```
  const envAdapter = () => {
  ```

- `src/components/SettingsSlider.tsx`:

  ```
  const SettingsNotDefined = () => {
  ```

## Use Solid's `createSignal` with `[value, setValue]` naming for reactive component state and SVG icons as zero-prop default-exported components.

- `src/components/Generator.tsx`:

  ```
  const [currentSystemRoleSettings, setCurrentSystemRoleSettings] = createSignal('')
  ```

- `src/components/icons/Clear.tsx`:

  ```
  export default () => {
  ```

- `src/components/icons/X.tsx`:

  ```
  export default () => {
  ```

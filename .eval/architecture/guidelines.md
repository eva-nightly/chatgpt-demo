# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## SolidJS components are exported as default anonymous arrow functions (no named function declarations), destructuring or receiving a typed `props` argument.

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

## Each component declares a module-local, non-exported `interface Props` immediately above the component to type its inputs rather than using inline or shared prop types.

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

## Read configuration through `import.meta.env` (Astro/Vite style, never `process.env`), providing a sensible fallback default with `||` where the variable is optional.

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

## Tooling configuration files use the framework's `defineConfig` helper and export it as the default export.

- `astro.config.mjs`:

  ```
  export default defineConfig({
  ```

- `unocss.config.ts`:

  ```
  export default defineConfig({
  ```

## Model shared data contracts as exported TypeScript `interface` declarations (e.g., chat messages, error payloads, auth payloads) rather than classes or type aliases.

- `src/types.ts`:

  ```
  export interface ChatMessage {
  ```

- `src/types.ts`:

  ```
  export interface ErrorMessage {
  ```

- `src/utils/auth.ts`:

  ```
  interface AuthPayload {
  ```

## Keep module-internal helpers as non-exported `const` arrow functions or plain functions scoped to the file, exporting only the public surface.

- `astro.config.mjs`:

  ```
  const envAdapter = () => {
  ```

- `plugins/disableBlocks.ts`:

  ```
  const transform = (code: string, id: string) => {
  ```

- `src/components/SettingsSlider.tsx`:

  ```
  const SettingsNotDefined = () => {
  ```

- `src/utils/auth.ts`:

  ```
  async function digestMessage(message: string) {
  ```

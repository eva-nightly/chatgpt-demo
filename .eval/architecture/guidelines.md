# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Solid components declare a file-local `interface Props` and accept typed props (destructured or as a `props` object) rather than inline prop types.

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

- `src/components/SystemRoleSettings.tsx`:

  ```
  export default (props: Props) => {
  ```

## UI components and icons are exported as anonymous default arrow functions; one component per file.

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

## Read configuration from `import.meta.env` (Astro/Vite style), never `process.env`, and provide `||` fallbacks for optional values at the read site.

- `src/pages/api/auth.ts`:

  ```
  const realPassword = import.meta.env.SITE_PASSWORD || ''
  ```

- `src/pages/api/auth.ts`:

  ```
  const passList = realPassword.split(',') || []
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

## Tooling config files use `export default defineConfig({...})` from the respective framework.

- `astro.config.mjs`:

  ```
  export default defineConfig({
  ```

- `unocss.config.ts`:

  ```
  export default defineConfig({
  ```

## Shared domain and payload shapes are defined as exported TypeScript interfaces in dedicated type files/modules instead of being duplicated inline.

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

## Ambient/global typings are added via declaration merging in `.d.ts` files (e.g., extending ImportMetaEnv or JSX HTMLAttributes) rather than casting at use sites.

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

## Reusable utilities and non-component modules use named `export const` arrow functions; default exports are reserved for components, configs and plugins.

- `src/components/Slider.tsx`:

  ```
  export const Slider = (selectProps: Props) => {
  ```

- `src/utils/openAI.ts`:

  ```
  export const model = import.meta.env.OPENAI_API_MODEL || 'gpt-3.5-turbo'
  ```

- `src/utils/openAI.ts`:

  ```
  export const generatePayload = (
  ```

- `plugins/disableBlocks.ts`:

  ```
  export default function plugin() {
  ```

## Internal helpers are kept as module-private `const` arrow functions or plain functions and not exported.

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

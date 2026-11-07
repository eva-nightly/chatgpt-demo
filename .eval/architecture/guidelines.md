# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Configuration files export a single default object produced by the framework's defineConfig helper.

- `astro.config.mjs`:

  ```
  export default defineConfig({
  ```

- `unocss.config.ts`:

  ```
  export default defineConfig({
  ```

## SolidJS components are exported as anonymous default arrow functions; declare their inputs in a local `interface Props` immediately above the component.

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

## Icon components are stateless, prop-less anonymous default exports returning inline SVG.

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

## Read server configuration through typed import.meta.env (declared in src/env.d.ts), supplying a fallback value with `||` where a default makes sense rather than using process.env.

- `src/env.d.ts`:

  ```
  interface ImportMetaEnv {
  ```

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

## Shared data shapes are declared as exported TypeScript interfaces in src/types.ts and reused across client and server code.

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

## Utility and helper modules expose named `export const` functions/values rather than default exports; default exports are reserved for components, configs, and plugins.

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

## Prefer `const` arrow functions for internal helpers and keep them module-private unless needed elsewhere.

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

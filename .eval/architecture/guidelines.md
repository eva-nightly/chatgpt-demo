# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Read all configuration from import.meta.env (Astro/Vite), never process.env, and provide sensible fallbacks with `||` where a default makes sense.

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

## Declare environment variable types in src/env.d.ts via ImportMetaEnv/ImportMeta interface augmentation so every env read is type-checked.

- `src/env.d.ts`:

  ```
  interface ImportMetaEnv {
  ```

- `src/env.d.ts`:

  ```
  interface ImportMeta {
  ```

## Config files export a single default `defineConfig({...})` object; keep env-dependent logic in small helper functions rather than inline in the config.

- `astro.config.mjs`:

  ```
  export default defineConfig({
  ```

- `unocss.config.ts`:

  ```
  export default defineConfig({
  ```

- `astro.config.mjs`:

  ```
  const envAdapter = () => {
  ```

## SolidJS components are anonymous arrow-function default exports that destructure (or accept) a locally declared `interface Props`; only utility components like Slider use named exports.

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

- `src/components/Slider.tsx`:

  ```
  export const Slider = (selectProps: Props) => {
  ```

## Define a local, non-exported `interface Props` at the top of each component file to type its inputs.

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

## Icon components live under src/components/icons as zero-prop anonymous default exports returning inline SVG.

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

## Shared data shapes (ChatMessage, ErrorMessage, AuthPayload) are declared as TypeScript interfaces; export them from src/types.ts when used across modules, keep them local otherwise.

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

## Prefer small, explicitly typed helper functions (e.g. transform, digestMessage, generatePayload) over inline logic in route handlers and plugins.

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

## Augment third-party JSX typings via a shims.d.ts that extends HTMLAttributes with AttributifyAttributes to support UnoCSS attributify mode.

- `shims.d.ts`:

  ```
  interface HTMLAttributes extends AttributifyAttributes { }
  ```

- `shims.d.ts`:

  ```
  interface HTMLAttributes<> extends AttributifyAttributes {}
  ```

## Manage reactive component state with Solid's createSignal tuples using the `[value, setValue]` naming convention.

- `src/components/Generator.tsx`:

  ```
  const [currentSystemRoleSettings, setCurrentSystemRoleSettings] = createSignal('')
  ```

- `src/components/Generator.tsx`:

  ```
  export default () => {
  ```

# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Read configuration through Vite/Astro `import.meta.env` (with sensible `|| ''` or default fallbacks), never `process.env`; declare every variable in `ImportMetaEnv` in src/env.d.ts.

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

- `src/env.d.ts`:

  ```
  interface ImportMetaEnv {
  ```

## Define component props as a local `interface Props` immediately above the component and destructure or accept `props: Props` in the signature.

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

## Export SolidJS components and icons as anonymous arrow-function default exports; use named exports only for reusable primitives like Slider.

- `src/components/Generator.tsx`:

  ```
  export default () => {
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

- `src/components/Slider.tsx`:

  ```
  export const Slider = (selectProps: Props) => {
  ```

## Share domain types via exported interfaces in src/types.ts (e.g., ChatMessage, ErrorMessage) and import them with the `@/` alias rather than redefining shapes per module.

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

## Config files (astro, unocss) use `export default defineConfig({...})`; build plugins export a default factory function returning a Vite plugin object with a `transform` hook.

- `astro.config.mjs`:

  ```
  export default defineConfig({
  ```

- `unocss.config.ts`:

  ```
  export default defineConfig({
  ```

- `plugins/disableBlocks.ts`:

  ```
  export default function plugin() {
  ```

- `plugins/disableBlocks.ts`:

  ```
  const transform = (code: string, id: string) => {
  ```

## Keep helper logic in small `const` arrow functions or `async function` helpers scoped to the file (e.g., adapter selection, signature digest, payload builders) and expose only the needed surface.

- `astro.config.mjs`:

  ```
  const envAdapter = () => {
  ```

- `src/utils/auth.ts`:

  ```
  async function digestMessage(message: string) {
  ```

- `src/utils/openAI.ts`:

  ```
  export const generatePayload = (
  ```

- `src/components/SettingsSlider.tsx`:

  ```
  const SettingsNotDefined = () => {
  ```

## Augment third-party JSX typings for UnoCSS attributify via ambient `interface HTMLAttributes extends AttributifyAttributes` declarations in shims.d.ts rather than inline casts.

- `shims.d.ts`:

  ```
  interface HTMLAttributes extends AttributifyAttributes { }
  ```

- `shims.d.ts`:

  ```
  interface HTMLAttributes<> extends AttributifyAttributes {}
  ```

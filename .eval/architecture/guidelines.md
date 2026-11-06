# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Export SolidJS components as anonymous default arrow functions; only use named exports for reusable primitives like Slider.

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

- `src/components/icons/X.tsx`:

  ```
  export default () => {
  ```

## Declare component props with a local `interface Props` directly above the component and destructure or accept it as the single parameter.

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

## Read configuration via typed `import.meta.env` (Astro/Vite style), never `process.env`, and provide sensible fallbacks with `||` where a default makes sense.

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

## Place shared data models in `src/types.ts` as exported interfaces and augment ambient types (ImportMetaEnv, ImportMeta, JSX HTMLAttributes) in `.d.ts` files.

- `src/env.d.ts`:

  ```
  interface ImportMetaEnv {
  ```

- `src/env.d.ts`:

  ```
  interface ImportMeta {
  ```

- `src/types.ts`:

  ```
  export interface ChatMessage {
  ```

- `src/types.ts`:

  ```
  export interface ErrorMessage {
  ```

- `shims.d.ts`:

  ```
  interface HTMLAttributes extends AttributifyAttributes { }
  ```

- `shims.d.ts`:

  ```
  interface HTMLAttributes<> extends AttributifyAttributes {}
  ```

## Configuration files use `export default defineConfig({...})`; build plugins export a default factory function with a separate `transform` helper.

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

## Manage client state with SolidJS `createSignal` pairs named `[value, setValue]` inside the component body.

- `src/components/Generator.tsx`:

  ```
  const [currentSystemRoleSettings, setCurrentSystemRoleSettings] = createSignal('')
  ```

- `src/components/Generator.tsx`:

  ```
  export default () => {
  ```

- `src/components/Slider.tsx`:

  ```
  export const Slider = (selectProps: Props) => {
  ```

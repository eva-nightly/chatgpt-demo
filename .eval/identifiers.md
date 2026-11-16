# Identifiers in this code

Every row is a `@uxid` comment in this repository: above a declaration (`// @uxid <id>`, `# @uxid <id>` in
Python), or for an element inside its opening tag (`<button /* @uxid <id> */ ...>`). Search the code for an
id to find its place, wherever the file has moved. Ids are permanent: never edit or remove one, and copy
none: a new component gets its own on Eva's next scan.

## Components (11)

| identifier | file | description |
| --- | --- | --- |
| `src/components/ErrorMessageItem::ErrorMessageItem` | src/components/ErrorMessageItem.tsx | Default-exported component. Props: data, onRetry. Renders: div, span, IconRefresh. |
| `src/components/Generator::Generator` | src/components/Generator.tsx | Default-exported component. Hooks: useThrottleFn. Renders: div, span, textarea, button, SystemRoleSettings, Index, MessageItem, ErrorMessageItem, +2 more. |
| `src/components/icons/Clear::Clear` | src/components/icons/Clear.tsx | Default-exported component. Renders: svg, path. |
| `src/components/icons/Env::Env` | src/components/icons/Env.tsx | Default-exported component. Renders: svg, path. |
| `src/components/icons/Refresh::Refresh` | src/components/icons/Refresh.tsx | Default-exported component. Renders: svg, path. |
| `src/components/icons/X::X` | src/components/icons/X.tsx | Default-exported component. Renders: svg, path. |
| `src/components/MessageItem::MessageItem` | src/components/MessageItem.tsx | Default-exported component. Props: role, message, showRetry, onRetry. Hooks: useClipboard, useEventListener. Renders: div, span, IconRefresh. |
| `src/components/SettingsSlider::SettingsNotDefined` | src/components/SettingsSlider.tsx | Arrow function component. Renders: div. |
| `src/components/SettingsSlider::SettingsSlider` | src/components/SettingsSlider.tsx | Default-exported component. Props: settings, editing, value, setValue. Renders: div, Slider, SettingsNotDefined. |
| `src/components/Slider::Slider` | src/components/Slider.tsx | Arrow function component. Props: props: Props. Hooks: useMachine. Renders: div, span, output, input. |
| `src/components/SystemRoleSettings::SystemRoleSettings` | src/components/SystemRoleSettings.tsx | Default-exported component. Props: props: Props. Renders: div, span, p, textarea, button, Show, IconEnv, IconX, +1 more. |

## Interactive elements (buttons, inputs, links), each inside a component (15)

| identifier | file | in | description |
| --- | --- | --- | --- |
| `src/components/ErrorMessageItem::ErrorMessageItem.div` | src/components/ErrorMessageItem.tsx | `src/components/ErrorMessageItem::ErrorMessageItem` | <div> element. Handlers: onClick. |
| `src/components/Generator::Generator.button` | src/components/Generator.tsx | `src/components/Generator::Generator` | Button. can be disabled, labelled "Send". Handlers: onClick. |
| `src/components/Generator::Generator.button-2` | src/components/Generator.tsx | `src/components/Generator::Generator` | Button. can be disabled, labelled "Clear". Handlers: onClick. |
| `src/components/Generator::Generator.button-3` | src/components/Generator.tsx | `src/components/Generator::Generator` | Button. type=button, labelled "stick to bottom". Handlers: onClick. |
| `src/components/Generator::Generator.div` | src/components/Generator.tsx | `src/components/Generator::Generator` | <div> element. labelled "Stop". Handlers: onClick. |
| `src/components/Generator::Generator.errormessageitem` | src/components/Generator.tsx | `src/components/Generator::Generator` | <ErrorMessageItem> component. Handlers: onRetry. |
| `src/components/Generator::Generator.messageitem` | src/components/Generator.tsx | `src/components/Generator::Generator` | <MessageItem> component. Handlers: onRetry. |
| `src/components/Generator::Generator.messageitem-2` | src/components/Generator.tsx | `src/components/Generator::Generator` | <MessageItem> component. |
| `src/components/Generator::Generator.textarea` | src/components/Generator.tsx | `src/components/Generator::Generator` | Multi-line text field. placeholder "Enter something...", can be disabled. Handlers: onKeyDown, onInput. |
| `src/components/MessageItem::MessageItem.div` | src/components/MessageItem.tsx | `src/components/MessageItem::MessageItem` | <div> element. Handlers: onClick. |
| `src/components/Slider::Slider.input` | src/components/Slider.tsx | `src/components/Slider::Slider` | Text input field. |
| `src/components/SystemRoleSettings::SystemRoleSettings.button` | src/components/SystemRoleSettings.tsx | `src/components/SystemRoleSettings::SystemRoleSettings` | Button. labelled "Set". Handlers: onClick. |
| `src/components/SystemRoleSettings::SystemRoleSettings.span` | src/components/SystemRoleSettings.tsx | `src/components/SystemRoleSettings::SystemRoleSettings` | <span> element. Handlers: onClick. |
| `src/components/SystemRoleSettings::SystemRoleSettings.span-2` | src/components/SystemRoleSettings.tsx | `src/components/SystemRoleSettings::SystemRoleSettings` | <span> element. Handlers: onClick. |
| `src/components/SystemRoleSettings::SystemRoleSettings.textarea` | src/components/SystemRoleSettings.tsx | `src/components/SystemRoleSettings::SystemRoleSettings` | Multi-line text field. placeholder "You are a helpful assistant, answer as concisely as possible....". |

## The code on the way to the AI: endpoint handlers and functions that call a model (2)

| identifier | file | description |
| --- | --- | --- |
| `src/pages/api/auth::post` | src/pages/api/auth.ts | Exported Function 'post'. Params: context. |
| `src/pages/api/generate::post` | src/pages/api/generate.ts | Exported Function 'post'. Params: context. |

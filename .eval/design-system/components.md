# Components

Every row is an applied `// @uxid` identifier. Ids are path-derived and permanent.

| identifier | file | flow | type | description |
| --- | --- | --- | --- | --- |
| `src/components/ErrorMessageItem::ErrorMessageItem` | src/components/ErrorMessageItem.tsx | all | component | Default-exported component. Props: data, onRetry. Renders: div, span, IconRefresh. |
| `src/components/Generator::Generator` | src/components/Generator.tsx | all | component | Default-exported component. Hooks: useThrottleFn. Renders: div, span, textarea, button, SystemRoleSettings, Index, MessageItem, ErrorMessageItem, +2 more. |
| `src/components/icons/Clear::Clear` | src/components/icons/Clear.tsx | all | component | Default-exported component. Renders: svg, path. |
| `src/components/icons/Env::Env` | src/components/icons/Env.tsx | all | component | Default-exported component. Renders: svg, path. |
| `src/components/icons/Refresh::Refresh` | src/components/icons/Refresh.tsx | all | component | Default-exported component. Renders: svg, path. |
| `src/components/icons/X::X` | src/components/icons/X.tsx | all | component | Default-exported component. Renders: svg, path. |
| `src/components/MessageItem::MessageItem` | src/components/MessageItem.tsx | all | component | Default-exported component. Props: role, message, showRetry, onRetry. Hooks: useClipboard, useEventListener. Renders: div, span, IconRefresh. |
| `src/components/SettingsSlider::SettingsNotDefined` | src/components/SettingsSlider.tsx | all | component | Arrow function component. Renders: div. |
| `src/components/SettingsSlider::SettingsSlider` | src/components/SettingsSlider.tsx | all | component | Default-exported component. Props: settings, editing, value, setValue. Renders: div, Slider, SettingsNotDefined. |
| `src/components/Slider::Slider` | src/components/Slider.tsx | all | component | Arrow function component. Props: props: Props. Hooks: useMachine. Renders: div, span, output, input. |
| `src/components/SystemRoleSettings::SystemRoleSettings` | src/components/SystemRoleSettings.tsx | all | component | Default-exported component. Props: props: Props. Renders: div, span, p, textarea, button, Show, IconEnv, IconX, +1 more. |

## Coverage

- all: 11 identifier(s)

## Design system components

11 component(s) carry a stable `@uxid`. 0 declare variants (0 axis/axes, 0 value(s) in total), read from `cva()` calls, class maps, prop unions and conditional class branches.

| @uxid | component | file | variants | states | uses | notes |
| --- | --- | --- | --- | --- | --- | --- |
| "src/components/ErrorMessageItem::ErrorMessageItem" | ErrorMessageItem | `src/components/ErrorMessageItem.tsx` |  |  | 0 | Renders a single error entry in the message flow, distinguishing failures from ordinary @src/components/MessageItem::MessageItem entries. |
| "src/components/Generator::Generator" | Generator | `src/components/Generator.tsx` |  |  | 0 | Top-level component that orchestrates the generation experience; the file name suggests it composes message items, settings, and controls, though the list does not detail its internals. |
| "src/components/MessageItem::MessageItem" | MessageItem | `src/components/MessageItem.tsx` |  |  | 0 | Displays one message in the conversation or output stream. |
| "src/components/SettingsSlider::SettingsNotDefined" | SettingsNotDefined | `src/components/SettingsSlider.tsx` |  |  | 0 | Fallback rendered by the settings slider file when a setting is not defined; exact behavior is not stated. |
| "src/components/SettingsSlider::SettingsSlider" | SettingsSlider | `src/components/SettingsSlider.tsx` |  |  | 0 | A settings-specific wrapper around @src/components/Slider::Slider for adjusting numeric configuration values. |
| "src/components/Slider::Slider" | Slider | `src/components/Slider.tsx` |  | disabled | 1 | The base range slider control; its thumb and track dimensions are governed by tokens t0 and t1 from src/slider.css. |
| "src/components/SystemRoleSettings::SystemRoleSettings" | SystemRoleSettings | `src/components/SystemRoleSettings.tsx` |  |  | 0 | Settings panel for defining the system role used by the generator. |
| "src/components/icons/Clear::Clear" | Clear | `src/components/icons/Clear.tsx` |  |  | 0 | Icon representing a clear action, presumably for resetting messages or input. |
| "src/components/icons/Env::Env" | Env | `src/components/icons/Env.tsx` |  |  | 0 | Icon named Env; its specific meaning is not stated in the list. |
| "src/components/icons/Refresh::Refresh" | Refresh | `src/components/icons/Refresh.tsx` |  |  | 0 | Icon representing a refresh or regenerate action. |
| "src/components/icons/X::X" | X | `src/components/icons/X.tsx` |  |  | 0 | Close/dismiss icon. |

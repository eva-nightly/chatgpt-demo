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
| "src/components/ErrorMessageItem::ErrorMessageItem" | ErrorMessageItem | `src/components/ErrorMessageItem.tsx` |  |  | 0 | A message list item dedicated to displaying an error state, as a counterpart to the standard message item. |
| "src/components/Generator::Generator" | Generator | `src/components/Generator.tsx` |  |  | 0 | The main generator component that hosts the product's core generate-and-display flow. |
| "src/components/MessageItem::MessageItem" | MessageItem | `src/components/MessageItem.tsx` |  |  | 0 | Renders a single message entry within the generated output. |
| "src/components/SettingsSlider::SettingsNotDefined" | SettingsNotDefined | `src/components/SettingsSlider.tsx` |  |  | 0 | A fallback rendered by the settings slider module when a setting has not been defined. |
| "src/components/SettingsSlider::SettingsSlider" | SettingsSlider | `src/components/SettingsSlider.tsx` |  |  | 0 | A settings control that wraps the slider primitive for adjusting a numeric setting. |
| "src/components/Slider::Slider" | Slider | `src/components/Slider.tsx` |  | disabled | 1 | The base slider primitive; its thumb and track dimensions are governed by t0 and t1 from src/slider.css. |
| "src/components/SystemRoleSettings::SystemRoleSettings" | SystemRoleSettings | `src/components/SystemRoleSettings.tsx` |  |  | 0 | A settings panel for configuring the system role used by the generator. |
| "src/components/icons/Clear::Clear" | Clear | `src/components/icons/Clear.tsx` |  |  | 0 | Icon representing a clear action. |
| "src/components/icons/Env::Env" | Env | `src/components/icons/Env.tsx` |  |  | 0 | Icon representing environment-related information or settings. |
| "src/components/icons/Refresh::Refresh" | Refresh | `src/components/icons/Refresh.tsx` |  |  | 0 | Icon representing a refresh or regenerate action. |
| "src/components/icons/X::X" | X | `src/components/icons/X.tsx` |  |  | 0 | Icon representing a close or dismiss action. |

# Design system playbook

Based on the component names, this product appears to be a chat-style generation interface: a Generator component drives the interaction, individual messages and error messages are rendered as list items, and a settings area exposes a system role input plus slider-based numeric controls. The only extracted tokens are two spacing tokens scoped to the slider (t0 for thumb size, t1 for track height, both from src/slider.css); no color, typography, or other token groups were listed, so the system as captured is small and slider-centric. A handful of simple icons (clear, env, refresh, close) support the controls.

## In one screen

- **Theme lives in:** plain CSS custom properties.
- **Tokens:** 2 in 1 group(s), folded from 2 declaration(s).
- **Themes:** light only.
- **Spent:** 2 token(s) are used somewhere; 0 are declared and never used.
- **Components:** 2 declared, 0 primitives, 0 with variants (0 variant value(s)).
- **Disagreements:** 27 instance(s) in 2 kind(s). See the last section.

## Where the design is declared

| file | what it declares |
| --- | --- |
| `src/slider.css`:12 | 2 custom properties declared under `[data-scope='slider'][data-part='control']`. |

## Palette

0 colour token(s) are re-declared for dark mode; 0 keep their light value.

## Scales

### Spacing

| step | expression | computed | uses | defined at |
| --- | --- | --- | --- | --- |
| `--slider-track-height` | `4px` | 4px | 2 | `src/slider.css`:14 |
| `--slider-thumb-size` | `14px` | 14px | 4 | `src/slider.css`:13 |

### Breakpoints

No breakpoint tokens are declared, so the framework defaults are in use. Responsive variants actually used: md (1).

### Typography

No font families or type steps are declared in the stylesheets.

## States the UI actually targets

| state | class occurrences |
| --- | --- |
| `dark` | 10 |
| `hover` | 10 |
| `placeholder` | 2 |
| `active` | 1 |
| `group-hover` | 1 |

## Composition

No primitives directory was found, so every component is an application component: there is an inventory here but no shared kit to build from.

## Where the app disagrees with itself

### 22 class(es) paint with Tailwind's stock palette instead of the token palette

18 distinct utilities, most used: bg-gray-200 (2), bg-gray-400 (2), bg-gray-600 (2), bg-neutral-300 (2), bg-gray-300 (1), bg-gray-500 (1), bg-gray-700 (1), bg-neutral-700 (1).

- `src/slider.css`:33: `bg-gray-200`
- `src/slider.css`:54: `bg-gray-200`
- `src/slider.css`:24: `bg-gray-400`
- `src/slider.css`:27: `bg-gray-400`
- `src/slider.css`:24: `bg-gray-600`
- `src/slider.css`:67: `bg-gray-600`
- `src/slider.css`:64: `bg-neutral-300`
- `src/slider.css`:67: `bg-neutral-300`

### 5 hardcoded colour literal(s) bypass the tokens

Written into a colour property or an arbitrary class value.

- `src/message.css`:2: `background-color: #64748b10;`
- `src/message.css`:16: `background-color: #64748b40;`
- `src/message.css`:25: `border-bottom: 2px solid #64748b40;`
- `astro.config.mjs`:31: `theme_color: '#212129',`
- `astro.config.mjs`:32: `background_color: '#ffffff',`

### Every hardcoded colour, by file

| file | literal | duplicates |
| --- | --- | --- |
| `src/message.css`:2 | `#64748b10` |  |
| `src/message.css`:16 | `#64748b40` |  |
| `src/message.css`:25 | `#64748b40` |  |
| `astro.config.mjs`:31 | `#212129` |  |
| `astro.config.mjs`:32 | `#ffffff` |  |

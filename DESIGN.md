---
version: alpha
name: Jajan
description: A playful design system for consumer apps. Coconut-cream ground, white cards with a hard ledge, raspberry buttons and the colors of jajan pasar.
colors:
  primary: "#D6336C"
  primary-hover: "#C22A60"
  primary-edge: "#9E1F4D"
  primary-foreground: "#FFFFFF"
  background: "#F8EEDB"
  foreground: "#3B2314"
  card: "#FFFFFF"
  card-foreground: "#3B2314"
  popover: "#FFFFFF"
  popover-foreground: "#3B2314"
  secondary: "#FCDCE7"
  secondary-foreground: "#9E1F4D"
  secondary-edge: "#F6B4C9"
  muted: "#F1E3C9"
  muted-foreground: "#7A5B45"
  accent: "#F1E3C9"
  accent-foreground: "#3B2314"
  destructive: "#C9351B"
  destructive-foreground: "#FFFFFF"
  destructive-edge: "#962510"
  success: "#48A85C"
  success-foreground: "#3B2314"
  warning: "#F2B134"
  warning-foreground: "#3B2314"
  pandan: "#48A85C"
  pandan-foreground: "#3B2314"
  pandan-edge: "#2B7F47"
  martabak: "#F2B134"
  martabak-foreground: "#3B2314"
  martabak-edge: "#C98A12"
  gula: "#8A562A"
  gula-foreground: "#FFFFFF"
  gula-edge: "#5E3818"
  cendol: "#7FD3B8"
  cendol-foreground: "#3B2314"
  cendol-edge: "#3FA487"
  border: "#E8D8BE"
  input: "#9B7B5C"
  ring: "#D6336C"
typography:
  display:
    fontFamily: Plus Jakarta Sans
    fontSize: 56px
    fontWeight: 800
    lineHeight: 60px
    letterSpacing: -0.03em
  h1:
    fontFamily: Plus Jakarta Sans
    fontSize: 40px
    fontWeight: 800
    lineHeight: 44px
    letterSpacing: -0.025em
  h2:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: 800
    lineHeight: 36px
    letterSpacing: -0.02em
  h3:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 30px
    letterSpacing: -0.015em
  title:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: 700
    lineHeight: 26px
    letterSpacing: -0.01em
  body:
    fontFamily: Plus Jakarta Sans
    fontSize: 17px
    fontWeight: 400
    lineHeight: 26px
  button:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: 700
    lineHeight: 24px
  small:
    fontFamily: Plus Jakarta Sans
    fontSize: 15px
    fontWeight: 400
    lineHeight: 22px
  ui:
    fontFamily: Plus Jakarta Sans
    fontSize: 15px
    fontWeight: 600
    lineHeight: 20px
  caption:
    fontFamily: Plus Jakarta Sans
    fontSize: 13px
    fontWeight: 600
    lineHeight: 16px
  price:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: 800
    lineHeight: 24px
    letterSpacing: -0.01em
rounded:
  xs: 8px
  sm: 12px
  md: 14px
  lg: 16px
  xl: 20px
  2xl: 24px
  3xl: 28px
spacing:
  "1": 4px
  "2": 8px
  "3": 12px
  "4": 16px
  "5": 20px
  "6": 24px
  "7": 28px
  "8": 32px
  "12": 48px
  "16": 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.primary-foreground}"
    borderColor: "{colors.primary-edge}"
    borderWidth: 2px
    shadow: "0 4px 0 0 {colors.primary-edge}"
    typography: "{typography.button}"
    rounded: "{rounded.lg}"
    height: 52px
    padding: 0 24px
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.secondary-foreground}"
    borderColor: "{colors.secondary-edge}"
    borderWidth: 2px
    shadow: "0 4px 0 0 {colors.secondary-edge}"
    typography: "{typography.button}"
    rounded: "{rounded.lg}"
    height: 52px
    padding: 0 24px
  button-ghost:
    textColor: "{colors.foreground}"
    typography: "{typography.button}"
    rounded: "{rounded.lg}"
    height: 52px
    padding: 0 24px
  button-ghost-hover:
    backgroundColor: "{colors.accent}"
  icon-button:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.input}"
    borderWidth: 2px
    shadow: "0 4px 0 0 {colors.input}"
    rounded: "{rounded.md}"
    size: 44px
  icon-button-quiet:
    textColor: "{colors.muted-foreground}"
    rounded: "{rounded.md}"
    size: 40px
  chip:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.input}"
    borderWidth: 2px
    shadow: "0 4px 0 0 {colors.input}"
    typography: "{typography.ui}"
    rounded: "{rounded.md}"
    height: 40px
    padding: 0 16px
  chip-selected:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.secondary-foreground}"
    borderColor: "{colors.primary}"
    shadow: "0 4px 0 0 {colors.primary}"
  toggle:
    backgroundColor: "{colors.muted}"
    borderColor: "{colors.input}"
    borderWidth: 2px
    shadow: "0 4px 0 0 {colors.input}"
    rounded: "{rounded.lg}"
    width: 72px
    height: 40px
  toggle-checked:
    backgroundColor: "{colors.primary}"
    borderColor: "{colors.primary-edge}"
    shadow: "0 4px 0 0 {colors.primary-edge}"
  stepper:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.input}"
    borderWidth: 2px
    shadow: "0 4px 0 0 {colors.input}"
    typography: "{typography.title}"
    rounded: "{rounded.lg}"
    height: 52px
  text-field:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.input}"
    borderWidth: 2px
    shadow: "0 4px 0 0 {colors.input}"
    typography: "{typography.body}"
    rounded: "{rounded.lg}"
    height: 52px
    padding: 0 16px
  badge:
    backgroundColor: "{colors.muted}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    typography: "{typography.caption}"
    rounded: "{rounded.md}"
    height: 32px
    padding: 0 12px
  sticker:
    backgroundColor: "{colors.martabak}"
    textColor: "{colors.martabak-foreground}"
    borderColor: "{colors.card}"
    borderWidth: 3px
    shadow: "0 0 0 2px {colors.martabak-edge}"
    typography: "{typography.caption}"
    rounded: "{rounded.md}"
    height: 36px
    padding: 0 12px
  avatar:
    backgroundColor: "{colors.pandan}"
    textColor: "{colors.pandan-foreground}"
    borderColor: "{colors.pandan-edge}"
    borderWidth: 2px
    typography: "{typography.ui}"
    rounded: "{rounded.md}"
    size: 44px
  toast:
    backgroundColor: "{colors.card}"
    textColor: "{colors.card-foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    shadow: "0 6px 0 0 {colors.border}"
    rounded: "{rounded.xl}"
    padding: 12px 8px 12px 16px
  card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.card-foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    shadow: "0 6px 0 0 {colors.border}"
    rounded: "{rounded.3xl}"
    padding: 20px
  product-card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.card-foreground}"
    borderColor: "{colors.border}"
    borderWidth: 2px
    shadow: "0 6px 0 0 {colors.border}"
    rounded: "{rounded.3xl}"
    padding: 8px 8px 12px
    width: 224px
---

# Jajan

## Overview

Jajan is a playful system for consumer apps: food ordering, pets, learning, kids, local communities. "Jajan" is Indonesian for buying snacks at a street stall or a market, and the whole look comes from jajan pasar, the traditional market snacks. The page is coconut cream, content sits on white cards with a 28px radius, text is deep palm-sugar brown, and the one main action is the raspberry pink of kue lapis. Pandan green, martabak yellow, palm-sugar brown and cendol mint color the categories, avatars, stickers and illustrations.

Every raised thing is a chunky rounded rectangle with a 2px border and a solid ledge, a hard bottom shadow in a darker shade of its own fill, like a piece of candy. Pressing a control sinks it onto its ledge. Targets are big: 52px controls, 40px chips, 44px icon buttons. Plus Jakarta Sans, heavy for headings, carries the text; the friendliness comes from the shapes around it, not from a novelty face.

The same tokens exist in three places and must stay in sync:

- `jajan.css` for Tailwind CSS v4. Token names follow shadcn/ui.
- This file, for people and coding agents.
- The Figma library "Jajan Design System" (variables, text styles, components).

When building with Jajan, use the semantic tokens and the recipes under Components. If a screen needs something this file does not cover, build it from the same parts: a white card or a cream panel, a 16px-radius control with a 2px border and a 4px ledge, 15px semibold interface text, and one raspberry element competing for attention.

## Colors

Use semantic tokens only. The default Tailwind palette is removed in `jajan.css`, so `bg-pink-500` and similar classes produce nothing. Every fill that can be raised has three shades: the fill, a `-foreground` for text on it, and an `-edge` for its border and ledge.

| Token | Light | Dark | Use |
| --- | --- | --- | --- |
| `background` | `#F8EEDB` | `#2A1911` | Page background: coconut cream, cocoa in the dark |
| `foreground` | `#3B2314` | `#FBF0DF` | Text and icons: palm sugar, cream in the dark |
| `card` | `#FFFFFF` | `#3B2314` | Cards, white controls, the thumb of a toggle |
| `card-foreground` | `#3B2314` | `#FBF0DF` | Text on cards |
| `popover` | `#FFFFFF` | `#3B2314` | Menus, popovers, dialogs, toasts |
| `popover-foreground` | `#3B2314` | `#FBF0DF` | Text on popovers |
| `primary` | `#D6336C` | `#D6336C` | The one main action; the on state of toggle, slider, radio, checkbox |
| `primary-hover` | `#C22A60` | `#C22A60` | Hover fill for primary |
| `primary-edge` | `#9E1F4D` | `#9E1F4D` | Border and ledge of primary fills |
| `primary-foreground` | `#FFFFFF` | `#FFFFFF` | Text on primary |
| `secondary` | `#FCDCE7` | `#55263A` | Secondary buttons, selected chips, selection |
| `secondary-foreground` | `#9E1F4D` | `#F6B4C9` | Text on secondary, and text-only actions such as Undo |
| `secondary-edge` | `#F6B4C9` | `#7E3656` | Border and ledge of secondary fills |
| `muted` | `#F1E3C9` | `#4A3425` | Picture panels, tracks, the off state of a toggle, badges |
| `muted-foreground` | `#7A5B45` | `#CDB49C` | Secondary text and resting icons |
| `accent` | `#F1E3C9` | `#4A3425` | Hover surface for ghost and quiet buttons |
| `accent-foreground` | `#3B2314` | `#FBF0DF` | Text on accent |
| `destructive` | `#C9351B` | `#D43B1F` | Errors and destructive actions: chili red, apart from the raspberry |
| `destructive-foreground` | `#FFFFFF` | `#FFFFFF` | Text on destructive |
| `destructive-edge` | `#962510` | `#962510` | Border and ledge of destructive fills |
| `success` | `#48A85C` | `#5DBE6E` | Success indicator; the same green as `pandan` |
| `success-foreground` | `#3B2314` | `#2A1911` | Text on success |
| `warning` | `#F2B134` | `#F5BD4A` | Warning indicator; the same yellow as `martabak` |
| `warning-foreground` | `#3B2314` | `#2A1911` | Text on warning |
| `pandan` | `#48A85C` | `#5DBE6E` | Category fill: klepon, dadar gulung, anything green |
| `pandan-foreground` | `#3B2314` | `#2A1911` | Text on pandan |
| `pandan-edge` | `#2B7F47` | `#2B7F47` | Border and outline of pandan shapes |
| `martabak` | `#F2B134` | `#F5BD4A` | Category fill: martabak manis, onde-onde, fried snacks |
| `martabak-foreground` | `#3B2314` | `#2A1911` | Text on martabak |
| `martabak-edge` | `#C98A12` | `#C98A12` | Border and outline of martabak shapes |
| `gula` | `#8A562A` | `#BD834D` | Category fill: palm sugar, chocolate, baskets |
| `gula-foreground` | `#FFFFFF` | `#2A1911` | Text on gula |
| `gula-edge` | `#5E3818` | `#8A562A` | Border and outline of gula shapes |
| `cendol` | `#7FD3B8` | `#7FD3B8` | Category fill: es cendol, drinks |
| `cendol-foreground` | `#3B2314` | `#2A1911` | Text on cendol |
| `cendol-edge` | `#3FA487` | `#3FA487` | Border and outline of cendol shapes |
| `border` | `#E8D8BE` | `#563D2B` | Border and ledge of cards, lists, panels, badges |
| `input` | `#9B7B5C` | `#8E7258` | Border and ledge of white controls: fields, chips, steppers, the off toggle |
| `ring` | `#D6336C` | `#F06292` | Focus ring |

`--radius` is `1rem`. Dark mode is the `.dark` class on a parent element.

Rules:

- One raspberry. `primary` is for the single main action of a view and for on or selected states. Headings, large surfaces and decoration never use it.
- The snack colors (`pandan`, `martabak`, `gula`, `cendol`) are for categories, avatars, stickers and illustrations. Each is used with its own `-foreground` and `-edge`; never put `foreground` or white on them by habit.
- `success` equals `pandan` and `warning` equals `martabak`, so a status and a category never fight. `destructive` is a chili red, clearly apart from the raspberry.
- Text on a white or cream surface is `foreground` or `muted-foreground`. Text-only actions (Undo, Change, links) are `secondary-foreground`, not `primary`: raspberry text passes AA only in light mode.
- `accent` is the hover surface, as in shadcn/ui. It is not a brand accent.

Measured contrast (WCAG 2.x ratios), light then dark:

- `foreground` on `background` 12.7 and 15.0; on `card` 14.6 and 13.0; on `muted` 11.5 and 10.3.
- `primary-foreground` on `primary` 4.6 in both modes; on `primary-hover` 5.5 in both.
- `secondary-foreground` on `secondary` 6.0 and 7.1; on `card` 7.6 and 8.6; on `background` 6.6 and 9.9.
- `muted-foreground` on `background` 5.4 and 8.5; on `card` 6.2 and 7.4; on `muted` 4.9 and 5.9; on `secondary` 4.9 and 6.2.
- `destructive-foreground` on `destructive` 5.2 and 4.7. Text on the snack fills: `pandan` 4.9 and 7.3, `martabak` 7.7 and 9.8, `gula` 6.1 and 5.2, `cendol` 8.3 and 9.6.
- Control boundaries (3:1 needed): `input` on `card` 3.9 and 3.3, on `background` 3.4 and 3.8; `primary` (the on state of a toggle) on `card` 4.6 and 3.2, on `background` 4.0 and 3.7; `ring` on `card` 4.6 and 4.8.

Every text pair above passes WCAG AA, and every control boundary passes 3:1. Two things fall short on purpose and have a rule: `primary` as text is 3.2:1 on the dark `card`, so text-only actions use `secondary-foreground` (7.6 and 8.6); and `border` is decorative (1.4:1 on white), so a card's outline is never the only thing that separates two states.

## Typography

Plus Jakarta Sans, loaded by the app (`next/font`, `@fontsource-variable/plus-jakarta-sans` or a link tag). Weights 400, 600, 700 and 800. It was made by Tokotype for Jakarta's city identity, which is where this system's name lives too.

| Utility | Size / line | Weight | Tracking | Use |
| --- | --- | --- | --- | --- |
| `type-display` | 56 / 60 | 800 | -0.03em | One per page at most |
| `type-h1` | 40 / 44 | 800 | -0.025em | Page title |
| `type-h2` | 32 / 36 | 800 | -0.02em | Section title, the wordmark |
| `type-h3` | 24 / 30 | 700 | -0.015em | Subsection, the letter of a large avatar |
| `type-title` | 20 / 26 | 700 | -0.01em | Card and dialog titles, product names, the stepper value |
| `type-body` | 17 / 26 | 400 | 0 | Body text, text inputs |
| `type-ui` | 15 / 20 | 600 | 0 | Chips, labels, list rows, card titles, small buttons |
| `type-small` | 15 / 22 | 400 | 0 | Option labels, hints, secondary text |
| `type-caption` | 13 / 16 | 600 | 0 | Badges, stickers and metadata |
| `type-price` | 18 / 24 | 800 | -0.01em | Prices, with tabular figures |

Buttons use `text-base font-bold` (16 / 24, weight 700).

Rules:

- Use the `type-*` utilities instead of composing size, weight and tracking by hand. They are not named `text-*` so that `tailwind-merge` does not confuse them with text colors.
- Interface text is `type-ui`, 15px semibold. Body copy is 17px. Reach for 13px only in badges and metadata.
- Prices are written the Indonesian way, `Rp12.000`, in `type-price`. Quantities next to a name are `type-small` in `muted-foreground`.
- Sentence case everywhere, including the wordmark, which is lowercase. No all caps.
- Text inputs stay at 17px so mobile browsers do not zoom on focus.

## Layout

- Spacing uses the Tailwind 4px unit. Common steps: 8 (inside a control), 12 (between stacked options), 16 (page margin, inside a text field), 20 (between cards, card padding), 24 (button padding).
- The page is `bg-background`. Content lives on white cards; the cream page is only ever a ground, with the page title and filters directly on it.
- Cards form a grid with `gap-5` and `p-4` page margins: one column on phones, two from 480px, three from 1024px. Gallery cards keep a 9:10 ratio (`aspect-[9/10]`).
- Big targets: default controls are 52px tall (`h-13`), small buttons and icon buttons 44px, chips 40px, toggles 72 by 40px, checkboxes and radios 24px. Never under 40px for anything a finger taps.
- Inside a card, the content is centered and the footer holds the title on the left and quiet icon buttons on the right.
- The ledge adds 4 or 6px below an element. Leave that room in stacked layouts: `gap-4` between buttons, `gap-5` between cards.

## Elevation & Depth

Depth is a ledge: a hard bottom shadow without blur in a darker shade of the fill, under a 2px border in the same shade. Nothing in the system is blurred, layered or translucent.

- Controls (buttons, fields, chips, toggles, steppers, raised icon buttons) have a 4px ledge: `ledge-primary-edge`, `ledge-secondary-edge`, `ledge-input`. The token is `--shadow-xs`.
- Cards, panels and toasts have a 6px ledge in `border`: `ledge-lg-border`. The token is `--shadow-sm`.
- Small raised parts that sit on a track, such as the selected segment and the slider thumb, have a 2px ledge: `ledge-sm-input`.
- Menus and dialogs have a 10px ledge in `border` (`--shadow-lg`) on top of the usual 2px border.
- Pressing sinks a control onto its ledge: `active:translate-y-1 active:shadow-none`. Ghost and quiet buttons have no ledge and only change color.
- Transitions are 120ms. The toggle thumb and stickers may use `ease-bounce`, a small overshoot. `prefers-reduced-motion` turns every transition and animation off in `jajan.css`.

## Shapes

Chunky rounded rectangles, never pills.

- Controls are `rounded-lg` (16px): buttons, fields, toggles, steppers.
- Chips, icon buttons, avatars and badges are `rounded-md` (14px). Checkboxes and the toggle thumb are `rounded-xs` (8px).
- Panels inside a card, lists and toasts are `rounded-xl` (20px). Cards are `rounded-3xl` (28px). A picture panel inside a card with `p-2` is `rounded-xl`, so the corners stay concentric.
- Circles are only for radios, status dots and the spinner's dots. No pill-shaped controls.
- Every fill has a 2px border in its `-edge` shade; white controls use `input`, white cards use `border`. Never a 1px line.

Icons are Lucide at 20px (`size-5`) with a 2.25 stroke in `currentColor`, round caps and joins. Icon-only buttons need an `aria-label`. Illustrations are built from the palette's shapes with `fill-*` and `stroke-*` utilities, 3px strokes in the `-edge` shade; no emoji and no gradients.

## Components

Copy these recipes. The live versions are in `preview/index.html`; every class is a token, a type utility or a ledge.

### Button

52px, 16px radius, 2px border and a 4px ledge in the fill's edge shade. One primary button per view.

```html
<button type="button" class="inline-flex h-13 items-center justify-center gap-2 rounded-lg border-2 px-6 text-base font-bold transition active:translate-y-1 active:shadow-none disabled:pointer-events-none disabled:opacity-40 border-primary-edge bg-primary text-primary-foreground ledge-primary-edge hover:bg-primary-hover">Add to basket</button>
```

- Secondary: replace the color classes with `border-secondary-edge bg-secondary text-secondary-foreground ledge-secondary-edge hover:bg-secondary-edge/40`.
- Ghost: `border-transparent text-foreground hover:bg-accent`, no ledge.
- Small (44px): `h-11 px-4 type-ui` instead of `h-13 px-6 text-base font-bold`.
- A leading 20px icon goes before the label; the `gap-2` is already there.

### Icon button

Raised, 44px, for actions on a card or in a header. Quiet, 40px, for rows and card footers.

```html
<button type="button" aria-label="Save Klepon" class="inline-flex size-11 items-center justify-center rounded-md border-2 border-input bg-card text-foreground ledge-input transition active:translate-y-1 active:shadow-none hover:bg-accent"><!-- 20px Lucide icon --></button>
```

- Quiet: `inline-flex size-10 items-center justify-center rounded-md text-muted-foreground transition hover:bg-accent hover:text-foreground`.
- Raspberry (the add button on a product card): `border-primary-edge bg-primary text-primary-foreground ledge-primary-edge hover:bg-primary-hover`.

### Stepper

Quantity control, 52px: a white control with a 4px ledge, a remove button, a tabular value and an add button. Disable the remove button at the minimum, and update a total next to it.

```html
<div role="group" aria-label="Quantity of Klepon" class="inline-flex h-13 items-center rounded-lg border-2 border-input bg-card ledge-input"><button type="button" aria-label="Remove one" class="inline-flex size-12 items-center justify-center text-foreground transition hover:bg-accent disabled:pointer-events-none disabled:opacity-40 rounded-l-md"><!-- minus --></button><output class="min-w-10 text-center type-title tabular-nums">2</output><button type="button" aria-label="Add one" class="inline-flex size-12 items-center justify-center text-foreground transition hover:bg-accent disabled:pointer-events-none disabled:opacity-40 rounded-r-md"><!-- plus --></button></div>
```

- On a product card the add button turns into a compact raspberry stepper (`h-11`, `border-primary-edge bg-primary text-primary-foreground ledge-primary-edge`, `size-10` buttons) and back when the count reaches zero.

### Chip

Filter chip, 40px, white with an `input` border and ledge. Selected: pink tint, raspberry border and ledge. Exactly one chip in a filter group has `aria-pressed="true"`.

```html
<button type="button" aria-pressed="false" class="inline-flex h-10 shrink-0 items-center gap-2 rounded-md border-2 border-input bg-card px-4 type-ui text-foreground ledge-input transition active:translate-y-1 active:shadow-none hover:bg-accent aria-pressed:border-primary aria-pressed:bg-secondary aria-pressed:text-secondary-foreground aria-pressed:ledge-primary aria-pressed:hover:bg-secondary">Sweet</button>
```

### Category chips

The same chip with a color dot in front: the snack color of the category. Several may be pressed at once.

```html
<button type="button" aria-pressed="true" class="inline-flex h-10 shrink-0 items-center gap-2 rounded-md border-2 border-input bg-card px-4 type-ui text-foreground ledge-input transition active:translate-y-1 active:shadow-none hover:bg-accent aria-pressed:border-primary aria-pressed:bg-secondary aria-pressed:text-secondary-foreground aria-pressed:ledge-primary aria-pressed:hover:bg-secondary"><span class="size-2.5 rounded-full bg-pandan"></span>Kue basah</button>
```

- Dots: `bg-pandan`, `bg-martabak`, `bg-cendol`, `bg-gula`. Give a category one color and keep it everywhere the category shows.

### Toggle

72 by 40px switch with a ledge: cream and `input` when off, raspberry and `primary-edge` when on. The thumb is a white rounded square that slides with a small bounce. Flip `aria-checked` on click; label it with `aria-labelledby`.

```html
<button type="button" role="switch" aria-checked="true" aria-labelledby="toggle-sugar" class="group relative h-10 w-18 rounded-lg border-2 border-input bg-muted ledge-input transition active:translate-y-1 active:shadow-none aria-checked:border-primary-edge aria-checked:bg-primary aria-checked:ledge-primary-edge disabled:opacity-40"><span class="absolute top-1 left-1 size-7 rounded-xs border-2 border-input bg-card transition-transform duration-200 ease-bounce group-aria-checked:translate-x-8 group-aria-checked:border-primary-edge"></span></button>
```

### Slider

A native range input with the `jajan-slider` utility from `jajan.css`: a 12px track with a 2px border, a raspberry fill and a 28px white thumb with a raspberry border and a 2px ledge. Chrome and Safari need `--slider-fill` to paint the filled part, so update it on every `input` event, and show the value in an `output`.

```html
<label class="block w-full max-w-60"><span class="flex justify-between type-ui">Sweetness<output class="text-muted-foreground tabular-nums">60%</output></span><input type="range" min="0" max="100" value="60" class="jajan-slider mt-2" /></label>
```

```js
el.style.setProperty('--slider-fill', `${((el.value - el.min) / (el.max - el.min)) * 100}%`);
```

### Single selection (radio)

Native radios in a `fieldset` with a `legend`. 24px, a 2px `input` border; checked is a raspberry fill with a white dot (`jajan-radio`).

```html
<label class="flex items-center gap-3 type-small"><input type="radio" name="fulfilment" checked class="size-6 appearance-none rounded-full border-2 border-input bg-card transition checked:border-primary-edge checked:bg-primary jajan-radio" />Pickup at 16:00</label>
```

Stack options with `space-y-3`; the legend is `type-ui mb-3`.

### Checkbox

The same as the radio, as a 24px rounded square with a white check (`jajan-check`).

```html
<label class="flex items-center gap-3 type-small"><input type="checkbox" checked class="size-6 appearance-none rounded-xs border-2 border-input bg-card transition checked:border-primary-edge checked:bg-primary jajan-check" />Extra grated coconut</label>
```

### Text field

52px, 16px radius, 2px `input` border and ledge, with a visible label above. The text is 17px.

```html
<label class="block w-full max-w-64"><span class="type-ui">Note for the seller</span><input type="text" placeholder="Extra grated coconut" class="mt-2 h-13 w-full rounded-lg border-2 border-input bg-card px-4 type-body text-foreground ledge-input placeholder:text-muted-foreground disabled:opacity-40" /></label>
```

For an error, add `aria-invalid="true"`, swap `border-input ledge-input` for `border-destructive ledge-destructive-edge`, and put a `type-small text-destructive` message below that says how to fix the value.

### Segmented control

A cream track with a 2px border; the selected segment is a raised white tab with a 2px ledge.

```html
<div role="tablist" aria-label="Fulfilment" class="inline-flex rounded-lg border-2 border-border bg-muted p-1"><button type="button" role="tab" aria-selected="true" class="h-10 rounded-sm border-2 border-transparent px-4 type-ui text-muted-foreground transition hover:text-foreground aria-selected:border-input aria-selected:bg-card aria-selected:text-foreground aria-selected:ledge-sm-input">Pickup</button></div>
```

### Badge

Status is a colored dot plus a word on a cream badge, never color alone.

```html
<span class="inline-flex h-8 items-center gap-2 rounded-md border-2 border-border bg-muted px-3 type-caption"><span class="size-2.5 rounded-full bg-success"></span>Open until 17:00</span>
```

- Dots: `bg-success`, `bg-warning`, `bg-destructive`.

### Sticker badge

A promotional label that sits on a product picture: a solid snack fill with a 3px white die-cut border and a 2px ring in the edge shade, tilted a few degrees.

```html
<span class="inline-flex h-9 items-center rounded-md border-[3px] border-card px-3 type-caption ring-2 -rotate-3 bg-martabak text-martabak-foreground ring-martabak-edge">Best seller</span>
```

- Other fills: `bg-pandan text-pandan-foreground ring-pandan-edge` (New), `bg-primary text-primary-foreground ring-primary-edge` (Save 20%). Tilt between -3 and 3 degrees, and never more than one sticker per picture.

### Progress

A 16px cream track with a 2px border and a raspberry fill. Say what is happening and how far, in words.

```html
<div class="w-full max-w-60"><div class="flex justify-between type-ui"><span>Packing your order</span><span class="text-muted-foreground tabular-nums">2 of 3</span></div><div role="progressbar" aria-label="Order progress" aria-valuenow="2" aria-valuemin="0" aria-valuemax="3" aria-valuetext="Packing, step 2 of 3" class="mt-2 h-4 overflow-hidden rounded-xs border-2 border-border bg-muted"><div class="h-full w-2/3 rounded-r-[4px] bg-primary"></div></div></div>
```

### Rating

Five radios in a `fieldset` with the `jajan-rating` utility: stars up to the checked one fill in martabak yellow with a darker outline. Arrow keys move the rating; the label shows the focus ring.

```html
<fieldset class="jajan-rating flex gap-1"><legend class="sr-only">Rate Klepon</legend><label class="cursor-pointer rounded-xs has-focus-visible:outline-3 has-focus-visible:outline-offset-2 has-focus-visible:outline-ring"><input type="radio" name="rating" value="1" class="sr-only" /><span class="sr-only">1 star</span><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linejoin="round" class="size-8 text-input transition" aria-hidden="true"><!-- Lucide star path --></svg></label></fieldset>
```

Repeat the label five times with values 1 to 5, and write the result next to it in `type-small`: "Klepon, 4 of 5".

### Avatar

A 44px rounded square in a snack color with one initial, a 2px edge border and a 2px `card` ring so a group can overlap.

```html
<span class="inline-flex size-11 items-center justify-center rounded-md border-2 type-ui ring-2 ring-card border-pandan-edge bg-pandan text-pandan-foreground">S</span>
```

- Group: `<div class="flex -space-x-3">` with up to four avatars and a count avatar in `border-border bg-muted text-muted-foreground`.
- Large: `size-16 rounded-lg type-h3`.

### List

Rows of 56px in a 20px-radius panel with 2px dividers. Prices sit right in tabular figures.

```html
<ul class="w-full max-w-64 divide-y-2 divide-border overflow-hidden rounded-xl border-2 border-border bg-card"><li class="flex h-14 items-center justify-between gap-3 px-4 type-ui tabular-nums"><span>Klepon <span class="text-muted-foreground">×2</span></span><span>Rp24.000</span></li></ul>
```

### Toast

A short confirmation with a pandan check and one text action. It is a 20px-radius panel with a 6px ledge; `role="status"` reads it out.

```html
<div role="status" class="flex w-full max-w-80 items-center gap-3 rounded-xl border-2 border-border bg-card py-3 pr-2 pl-4 ledge-lg-border"><span class="inline-flex size-9 shrink-0 items-center justify-center rounded-sm border-2 border-pandan-edge bg-pandan text-pandan-foreground"><!-- check --></span><p class="flex-1 type-ui">Klepon added to your basket</p><button type="button" class="h-10 shrink-0 rounded-md px-3 type-ui text-secondary-foreground transition hover:bg-accent">Undo</button></div>
```

### Empty state

An illustration built from the palette's shapes, a title, one line of help and a secondary button. The basket below is `gula` with `gula-edge` strokes and a `muted` shadow.

```html
<div class="flex flex-col items-center text-center"><svg viewBox="0 0 120 96" class="h-24" aria-hidden="true"><ellipse cx="60" cy="90" rx="42" ry="5" class="fill-muted"/><path d="M38 40C38 16 82 16 82 40" class="stroke-gula-edge" stroke-width="5" fill="none" stroke-linecap="round"/><path d="M22 42h76l-8 42q-30 6-60 0z" class="fill-gula stroke-gula-edge" stroke-width="3" stroke-linejoin="round"/><path d="M29 56h62M27 70h58" class="stroke-gula-edge" stroke-width="2.5" opacity=".45"/><rect x="18" y="36" width="84" height="12" rx="6" class="fill-gula-edge"/></svg><h3 class="mt-4 type-title">Your basket is empty</h3><p class="mt-1 type-small text-muted-foreground">Snacks you add show up here.</p><button type="button" class="inline-flex h-11 items-center justify-center gap-2 rounded-lg border-2 border-secondary-edge bg-secondary px-4 type-ui text-secondary-foreground ledge-secondary-edge transition active:translate-y-1 active:shadow-none hover:bg-secondary-edge/40 mt-4">Browse snacks</button></div>
```

### Spinner

Three snack-colored dots that hop in turn (`jajan-hop`). It stops under `prefers-reduced-motion`.

```html
<span role="status" aria-label="Loading" class="inline-flex items-end gap-2"><span class="jajan-hop size-4 rounded-full bg-pandan"></span><span class="jajan-hop size-4 rounded-full bg-primary [animation-delay:150ms]"></span><span class="jajan-hop size-4 rounded-full bg-martabak [animation-delay:300ms]"></span></span>
```

### Product card

A 224px card: a cream picture panel with an illustration made of shapes, the name with the portion in `type-small`, the price in rupiah and a raspberry add button. The name's quantity, the price and the button are the whole offer; no description.

```html
<article class="w-56 rounded-3xl border-2 border-border bg-card p-2 pb-3 ledge-lg-border"><div class="flex aspect-[16/10] items-center justify-center rounded-xl bg-muted"><!-- illustration: fill-pandan stroke-pandan-edge circles with fill-white speckles on a fill-card plate --></div><div class="px-2 pt-3"><h3 class="type-title">Klepon <span class="type-small text-muted-foreground">5 pcs</span></h3><div class="mt-3 flex items-center justify-between"><span class="type-price">Rp12.000</span><button type="button" aria-label="Add Klepon to basket" class="inline-flex size-11 items-center justify-center rounded-md border-2 border-primary-edge bg-primary text-primary-foreground ledge-primary-edge transition active:translate-y-1 active:shadow-none hover:bg-primary-hover"><!-- plus --></button></div></div></article>
```

### Card

White, 28px radius, 2px `border` and a 6px ledge. Content cards have `p-5`; gallery cards center their content and keep a footer.

```html
<article class="w-full max-w-64 rounded-3xl border-2 border-border bg-card p-5 ledge-lg-border"><p class="type-caption text-muted-foreground">Pickup</p><h3 class="mt-1 type-title">Today at 16:00</h3><p class="mt-1 type-small text-muted-foreground">Pasar Antri, stall 12. Show your order code at the stall.</p><button type="button" class="inline-flex h-11 items-center justify-center gap-2 rounded-lg border-2 border-secondary-edge bg-secondary px-4 type-ui text-secondary-foreground ledge-secondary-edge transition active:translate-y-1 active:shadow-none hover:bg-secondary-edge/40 mt-4">Change time</button></article>
```

Gallery card: `flex aspect-[9/10] flex-col rounded-3xl border-2 border-border bg-card ledge-lg-border`, a centered demo area with `px-6 pt-6`, and a 64px footer with the title in `type-ui` and quiet icon buttons.

### Focus

Every interactive element gets the global focus ring from `jajan.css`: a 3px `ring` outline with a 2px offset, raspberry in light mode and a lighter pink in the dark. Do not remove it. Controls whose input is visually hidden (the rating) draw it on their label with `has-focus-visible:outline-ring`.

## Do's and Don'ts

- Do give every raised control a 2px border and a ledge in the darker shade of its own fill, and sink it on press with `active:translate-y-1 active:shadow-none`.
- Do keep one primary button per view. A second action is secondary or ghost.
- Do use the snack colors for categories, avatars, stickers and illustrations, each with its own `-foreground` and `-edge`.
- Do pair every status color with a word, and write prices as `Rp12.000`.
- Do keep targets big: 52px controls, 44px icon buttons, 40px chips, 24px checkboxes.
- Do give icon-only buttons an `aria-label` and form controls a visible label.
- Don't use pills. The largest radius on a control is 16px; only radios, dots and the spinner are circles.
- Don't blur, layer or tint shadows. Depth is one hard ledge.
- Don't put raspberry text on dark surfaces; text actions are `secondary-foreground`.
- Don't use the default Tailwind palette, hard-coded hex values, gradients or emoji.
- Don't shrink interface text below 13px or text inputs below 16px.

# Changelog

Jajan uses semantic versions. While it is in beta, a minor version adds or changes tokens, components or rules,
and a patch fixes them. Every version is a git tag (`v0.1.0`) and an entry in the design site's record.

## 0.2.2 (2026-10-24)

For screen readers; nothing looks different.

- The gallery's title, jajan, is its `h1`.
- The Figma library does not change.

## 0.2.1 (2026-10-15)

- The gallery has no filter row under the header any more. Its 24 cards are grouped under category headings
  (Content, Actions, Inputs, Status) in `type-h3`, with 40px between groups and 20px under each heading; card
  names are `h3`. Copy, reset and every control work as before.
- Figma: the filter chip row is gone from `Gallery/Light` and `Gallery/Dark`.

## 0.2.0 (2026-10-14)

A blank component sheet and an example screen.

- The gallery in `preview/index.html` is a blank template: every component shows neutral content ("Save",
  "Email", "Option A", "Active / Pending / Failed / Draft", "Product name") instead of a snack shop's, with its
  variants and states. 24 live components, copy on every card and reset on the 12 that keep state. Gallery
  cards in a row now share one height.
- `preview/demo.html`, an example screen: the order page of a snack stall, built only from the recipes (17 kinds
  of component), in light and dark. It works: steppers, category chips, search, pickup or delivery, the toast
  with undo, the toggle and the rating.
- `DESIGN.md` has 24 recipes. New: Button sizes and Text field states, the Destructive button, disabled
  toggles, radios, checkboxes and sliders, the Draft badge, the list row with a chevron, and a product card with
  a short description and a compact stepper. The recipe markup is the gallery's.
- Fix: an error message is set in `foreground` with a red alert icon, because `destructive` as text is 3.1:1 on
  the dark card. The compact stepper's buttons get a white inset focus ring, since the raspberry ring did not
  show on the raspberry fill.
- Figma: neutral text in the components, the galleries and the cover. Button has 24 variants (Destructive and
  Disabled added); Toggle, Single selection and Checkbox have a Disabled variant; Text field has Disabled and an
  error message with an alert icon; Badge has Draft; Product card is a set with Added true and false, a
  swappable picture and an optional sticker; 10 picture components, and the icons circle-alert and search.
  A new page Example holds the demo screen as `Example/Light` and `Example/Dark`, 1280 wide, built from
  instances.

## 0.1.0 (2026-10-14)

First beta.

- Tokens in light and dark mode, in `jajan.css` (Tailwind CSS v4, shadcn/ui token names plus the snack colors
  `pandan`, `martabak`, `gula` and `cendol`, each with a `-foreground` and an `-edge`) and in the front matter
  of `DESIGN.md`.
- `DESIGN.md` with the rules, the measured contrast of both modes and 22 recipes.
- A component gallery in `preview/` with 22 live components, category filters, copy on every
  card and reset on the 11 that keep state: a snack shop's kit with Indonesian snacks and prices in rupiah.
- The Figma library "Jajan Design System": 111 variables in four collections, 12 text styles bound to the font
  variables, 9 ledge effect styles, 22 components (13 sets with 55 variants and 9 single components), 13 Lucide
  icons, and a light and a dark gallery built from instances.

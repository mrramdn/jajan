# Changelog

Jajan uses semantic versions. While it is in beta, a minor version adds or changes tokens, components or rules,
and a patch fixes them. Every version is a git tag (`v0.1.0`) and an entry in the design site's record.

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

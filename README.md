# Jajan

A playful design system for consumer apps: food ordering, pets, learning, kids, local communities. Coconut-cream ground, white cards with a hard ledge, raspberry buttons and the colors of jajan pasar. The same tokens exist as a Tailwind CSS v4 theme, a `DESIGN.md` that people and coding agents follow, and a Figma library.

"Jajan" is Indonesian for buying snacks at a street stall or a market. It is a working name.

## Files

| File | What it is |
| --- | --- |
| `jajan.css` | Tailwind CSS v4 theme: color tokens (light and dark), radii, ledge shadows, type utilities, the `ledge-*`, slider, checkbox, radio and rating utilities. Token names follow shadcn/ui. |
| `DESIGN.md` | The rules and the component recipes, in the [design.md](https://github.com/google-labs-code/design.md) format. |
| `preview/index.html` | Component gallery built with the theme: every component with neutral content, its variants and its states. Cards are grouped under category headings. Has a dark mode switch and copy and reset buttons per component. |
| `preview/demo.html` | An example screen built only from the recipes: the order page of a snack stall, with a menu, a cart and a rating. Light and dark follow the `dark` class. |
| `CHANGELOG.md` | What changed in each version. |
| `scripts/` | `check-version.mjs` (`pnpm check`: every place that names the version agrees) and `banner-first.mjs` (run by `pnpm build`: the theme's `/*!` banner stays line 1 of `preview/preview.css`). |
| `LICENSE` | MIT for `jajan.css` and everything in `preview/`; CC BY 4.0 for `DESIGN.md` and the Figma library. |

Figma: [Jajan Design System](https://www.figma.com/design/hL69pjHba5YSr9C127KJT7) (pages Cover, Foundations, Components and Example; Example holds the demo screen in light and dark).

## Use it in a project

1. Load Plus Jakarta Sans, weights 400 to 800 (for example `pnpm add @fontsource-variable/plus-jakarta-sans` and import it, or `next/font`).
2. Copy `jajan.css` next to your main stylesheet and import it after Tailwind:

   ```css
   @import "tailwindcss";
   @import "./jajan.css";
   ```

3. Copy `DESIGN.md` to the project root so coding agents follow the same rules.
4. Dark mode is the `.dark` class on `<html>`.

The theme removes the default Tailwind color palette on purpose. Use the semantic tokens (`bg-card`, `text-muted-foreground`, `bg-primary`, `bg-pandan` and so on). Depth is the `ledge-<color>` utilities: a hard bottom shadow in a darker shade of the fill, pressed away with `active:translate-y-1 active:shadow-none`.

## Preview

```sh
pnpm install
pnpm build   # writes preview/preview.css from the classes in preview/index.html and preview/demo.html
pnpm dev     # same, watching for changes
```

Then open `preview/index.html` (the gallery) or `preview/demo.html` (the example screen) in a browser. Copy needs a secure context, so serve the folder (`python3 -m http.server -d preview`) if the clipboard button does nothing over `file://`.

## Versions

The version is in `package.json`, `CHANGELOG.md` says what changed, and every release is a git tag. To release:

1. Change the files and run `pnpm build`, so `preview/preview.css` matches.
2. Raise the version everywhere it is written: `version` in `package.json`, a new entry at the top of `CHANGELOG.md`,
   the `/*!` banner on line 1 of `jajan.css` and `preview/input.css`, and `--jajan-build` in `jajan.css`'s `:root`.
   Run `pnpm build` again and `pnpm check`, which fails while any of them differ.
3. Commit, tag `v<version>` (`git tag -a v0.3.0 -m "Jajan 0.3.0"`) and push with `git push --follow-tags`, then
   publish a GitHub Release from the tag with the CHANGELOG entry.
4. On the design site, run `pnpm sync:system jajan <this folder>`, put the pictures in
   `public/images/jajan/<version>/`, and add the version to the record. The site's tests fail while the record, the
   synced files or a version the gallery names disagree.
5. Optionally, after the site deploys, save a Wayback snapshot of the product page in both languages.

## Licence

The code is MIT: `jajan.css` and everything in `preview/` (HTML and CSS). `DESIGN.md` and the Figma library "Jajan
Design System" are CC BY 4.0: copy and adapt them, also commercially, with credit: "Jajan by Rifki Ramdani,
https://uiux.mrramdn.com/en/systems/jajan". The full text is in [`LICENSE`](LICENSE).

## Where the look comes from

The palette is taken from the traditional market snacks: kue lapis (the raspberry pink of the layered cake), klepon and dadar gulung (pandan green), martabak manis (golden yellow), gula aren (palm sugar brown), es cendol (mint) and grated coconut (cream and white). The shapes are chunky rounded rectangles with a 2px border and a solid ledge in a darker shade, like candy. Plus Jakarta Sans is by Tokotype, an Indonesian foundry, made for Jakarta's city identity. The look is original; nothing is measured from another product.

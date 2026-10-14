# Jajan

A playful design system for consumer apps: food ordering, pets, learning, kids, local communities. Coconut-cream ground, white cards with a hard ledge, raspberry buttons and the colors of jajan pasar. The same tokens exist as a Tailwind CSS v4 theme, a `DESIGN.md` that people and coding agents follow, and a Figma library.

"Jajan" is Indonesian for buying snacks at a street stall or a market. It is a working name.

## Files

| File | What it is |
| --- | --- |
| `jajan.css` | Tailwind CSS v4 theme: color tokens (light and dark), radii, ledge shadows, type utilities, the `ledge-*`, slider, checkbox, radio and rating utilities. Token names follow shadcn/ui. |
| `DESIGN.md` | The rules and the component recipes, in the [design.md](https://github.com/google-labs-code/design.md) format. |
| `preview/index.html` | Component gallery built with the theme: a snack shop's kit. Has a dark mode switch, category filters, and copy and reset buttons per component. |
| `CHANGELOG.md` | What changed in each version. |

Figma: [Jajan Design System](https://www.figma.com/design/hL69pjHba5YSr9C127KJT7) (pages Cover, Foundations and Components).

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
pnpm build   # writes preview/preview.css from the classes in preview/index.html
pnpm dev     # same, watching for changes
```

Then open `preview/index.html` in a browser. Copy needs a secure context, so serve the folder (`python3 -m http.server -d preview`) if the clipboard button does nothing over `file://`.

## Versions

The version is in `package.json`, `CHANGELOG.md` says what changed, and every release is a git tag. To release:

1. Change the files and run `pnpm build`, so `preview/preview.css` matches the gallery.
2. Raise `version` in `package.json` and add an entry to `CHANGELOG.md`.
3. Commit, tag `v<version>` (`git tag -a v0.2.0 -m "Jajan 0.2.0"`) and push with `git push --follow-tags`.
4. On the design site, sync this folder and add the version to Jajan's record. The site's tests fail while the
   record states a different version from the synced files.

## Where the look comes from

The palette is taken from the traditional market snacks: kue lapis (the raspberry pink of the layered cake), klepon and dadar gulung (pandan green), martabak manis (golden yellow), gula aren (palm sugar brown), es cendol (mint) and grated coconut (cream and white). The shapes are chunky rounded rectangles with a 2px border and a solid ledge in a darker shade, like candy. Plus Jakarta Sans is by Tokotype, an Indonesian foundry, made for Jakarta's city identity. The look is original; nothing is measured from another product.

# Artwork folder

Scanned paintings go here. Nothing breaks while a file is missing — the site
just skips that image.

Filenames the site currently points at:

| File | Where it's referenced |
|---|---|
| `background.jpg` | `--bg-image` in `assets/css/style.css` (set it to turn the background on) |
| `logo.png` | `_includes/header.html` |
| `divider.png` | `--divider-image` in `assets/css/style.css` |
| `favicon.png` | `_layouts/default.html` |
| `icon-1.png`, `icon-2.png`, `icon-3.png` | `index.html` cards |

Reference any other image from a page or post as
`/assets/images/your-file.jpg`.

Two things that will bite you otherwise:

- **Filenames are case-sensitive on the live site but not on your Mac.**
  `Logo.png` works locally and 404s in production. Keep everything lowercase.
- **Large files make the site slow on phones.** Keep the background under
  roughly 800 KB.

Delete this file when you don't need it.

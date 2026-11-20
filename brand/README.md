# Helix brand assets

The official Helix logos. Use these files as they are: don't redraw, recolour or stretch them.

| File | What it is | Use it for |
|---|---|---|
| [`helix-mark.svg`](helix-mark.svg) | The mark alone, framed in a square | Icons, favicons, avatars, small spaces |
| [`helix-mark-512.png`](helix-mark-512.png) | The mark as a 512×512 PNG | Places that don't take SVG (the GitHub organization avatar, social profiles) |
| [`helix-logo-vertical.svg`](helix-logo-vertical.svg) | The mark above the "Helix" wordmark | Light backgrounds: READMEs, documents, the website in light mode |
| [`helix-logo-vertical-dark.svg`](helix-logo-vertical-dark.svg) | The same, with the wordmark in a light ink | Dark backgrounds |
| [`helix-x-cover.png`](helix-x-cover.png) | A 1500×500 banner: the mark, the wordmark and the tagline on a light background | The X (Twitter) header image, and other social banners |
| [`helix-x-profile.png`](helix-x-profile.png) | A 400×400 profile picture: the mark on the same background, with room for a circular crop | The X profile picture, and other social profiles |

The `.svg` files next to the two social images are their sources. The banner's tagline is set in Ubuntu Sans, so render it on a system that has that font (`rsvg-convert -w 1500 -h 500 helix-x-cover.svg -o helix-x-cover.png`).

The mark keeps its colours on both light and dark backgrounds. Only the wordmark changes for dark backgrounds.

## Colours

| Colour | Hex |
|---|---|
| Deep indigo (wordmark, darkest blade) | `#17194f` |
| Indigo | `#313a75` |
| Slate indigo | `#49518b` |
| Periwinkle | `#626aa3` |
| Wordmark on dark backgrounds | `#e6e8f6` |

## In the code

- **desktop:** the mark is installed as the `org.helixdesktop.Helix` icon (`data/icons/`), and the login screen shows it.
- **apps:** the Tour's welcome page shows the mark.
- **web:** the favicon, the site header and the homepage use these files (`public/`).

The logos are released under [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/), like the rest of Helix. The name "Helix" and the logos still identify this project, so please don't use them in a way that suggests your project is Helix or is endorsed by it.

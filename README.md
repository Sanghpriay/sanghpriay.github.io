# Portfolio Site

Source for [sanghpriay.github.io](https://sanghpriay.github.io) — a single static page
covering four analytics projects (optimisation, classical ML, applied GenAI, applied
statistics + deep learning), each linking to its own GitHub repo.

No build step — plain HTML/CSS, deployed directly via GitHub Pages.

## Structure

```
index.html   — all page content
style.css    — all styling
fonts/       — self-hosted IBM Plex Sans/Mono (SIL Open Font License, see fonts/LICENSE.txt)
```

Fonts are self-hosted rather than loaded from Google Fonts, so the page renders correctly
regardless of ad blockers, privacy extensions, or network restrictions that block third-party
font CDNs.

## Editing

To add or update a project, copy an existing `<article class="project-card">` block in
`index.html` and adjust the tag, headline result, description, tech tags, and repo link.
Colours, type, and spacing are all controlled via CSS custom properties at the top of
`style.css` (`:root { ... }`) if you want to restyle.

## Deploying updates

Since this repo is named `<username>.github.io`, GitHub Pages serves it automatically
from the `main` branch — just commit and push, and the live site updates within a
minute or two. No separate build or deploy step needed.

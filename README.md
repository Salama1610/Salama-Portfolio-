# salama

Portfolio site for **Abdelrahman Salama Ahmed** — Junior Project & Programme Manager.

A single static page. No build step, no dependencies, no framework: one `index.html`
with its CSS and JS inline, an `assets/` folder, and the CV as a PDF at the root.
Open `index.html` in a browser to work on it locally.

```
index.html                    the whole page
assets/                       photos, partner logos, OG image, favicon
Abdelrahman-Salama-CV.pdf     what the "Download PDF" button serves
vercel.json                   clean URLs, cache headers, download header
robots.txt, sitemap.xml       indexing
```

## The one rule

Every figure on this page is reconciled against the round reports. A number in a
metric tile is a claim: if it cannot survive a follow-up question, it does not go
in a tile. Programme-wide totals are never presented as individually delivered —
each project tab carries only its own figures.

## Deploying

Pushed to `main` and deployed by Vercel on every push. Nothing to build:
Framework Preset **Other**, no build command, output directory `./`.

## Editing

- **A number** — change it in the project tab *and* in the `#cv` section *and* in
  the PDF; the three must agree.
- **A partner logo** — drop a transparent PNG in `assets/`, rendered at 3× the CSS
  height. Dark neutral ink is recoloured to near-white and dark brand colour is
  lifted by its max channel so the hue survives on a near-black ground. Keep the
  wordmark: a partner is recognised by its name, not its glyph.
- **A photo** — any aspect ratio; the gallery crops to 4:3 cards. Export at about
  780px on the long edge, quality 82.
- **A project** — copy a `.panel` block, add its `.tab` button, and keep the tab
  and panel ids in step (`t5` ↔ `p5`).

## Theme

Dark by decision: the work is read at night by people scanning many candidates,
and a dark ground lets the figures carry the page. Tokens live in `:root`.

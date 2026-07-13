# Xprotocols-lab / STITCH

Jekyll site with the exact same setup as axi-security.github.io (dev-2-branch): `minima`-based theme, custom `_layouts` (default, home, page, post, and a project layout — `stitch.html`, adapted from their `expect.html`/`xray.html` pattern), shared `_includes` (header, footer, icons, bibtex popup), and the same `_sass` structure.

## Structure

```
_config.yml        site title/url/email
_layouts/          default.html, home.html, page.html, post.html, stitch.html
_includes/         header.html, footer.html, head.html, social.html, icon-*.svg, bibtex-popup.html
_sass/             minima.scss + minima/_base.scss, _layout.scss, _syntax-highlighting.scss
assets/            main.scss (compiles the sass), implementation_logo.png
stitch/index.md    the paper's content page (layout: stitch)
index.md           home page linking to /stitch/
```

## Run locally / deploy

Requires Ruby + Bundler (same as the original repo).

```
bundle install
bundle exec jekyll serve
```

To deploy on GitHub Pages: push this folder's contents to the root of `Xprotocols-lab/STITCH`, then enable Pages (Settings → Pages → Deploy from a branch → `main` / `root`). GitHub Pages builds Jekyll automatically — no manual build step needed.

## Editing content

Edit `stitch/index.md` for the abstract/contributions copy, and `_layouts/stitch.html` for the authors list, venue, and GitHub/PDF links (currently placeholders — update the PDF link once you upload `assets/stitch_dac26.pdf`). Swap `assets/implementation_logo.png` for real per-contribution icons whenever you have them.

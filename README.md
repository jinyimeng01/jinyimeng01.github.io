# HaiTang — Jianhe Li · Personal Homepage

Personal website of **Jianhe Li** (李建赫), security researcher focused on
**Web AI security** and **binary security**.

**Live:** <https://jinyimeng01.github.io/HaiTang/>

Built with [Jekyll](https://jekyllrb.com) on the
[Academic Pages](https://academicpages.github.io/) template (a fork of
Minimal Mistakes), with a custom Apple-style **glass theme** layered on top.

---

## What's customized

- **`assets/css/glass.css`** — the entire glassmorphism overlay: flowing aurora
  background, glass cards / buttons / nav, two-column layout, typography.
  Append-only over the theme's `_sass/`.
- **Animated metallic gradient + 3 swappable palettes** — driven by the
  `--grad-premium` CSS variable; the `grad-flow` keyframe sweeps a metallic
  highlight band across gradient text. A bottom-right switcher (built by JS in
  `_includes/head/custom.html`) toggles `body.theme-aurora|haitang|onyx` and
  persists the choice in `localStorage`. Default = **Aurora**
  (ink-blue + deep-purple + platinum).
- **`_includes/author-profile.html`** — added a WeChat link (click-to-copy via
  `data-copy`); removed the non-functional "Follow" button.
- **`_layouts/single.html`** — suppress the redundant `<h1>` title on the
  homepage only.
- **`_includes/head/custom.html`** — links `glass.css` (cache-busted per build
  via `?v=<timestamp>`), click-to-copy script, gradient-theme switcher.
- **`_includes/footer/custom.html`** — MathJax loader.
- **Official SVG logos** in `images/logos/` (Microsoft / Intel / Google / Apple)
  — hand-coded vectors, no external image dependency.
- **Avatar** — `images/profile.jpg`.

## Content map

| What | Where |
|---|---|
| Identity, social links, timezone | `_config.yml` (`title`, `name`, `author:`) |
| Homepage copy & section order | `_pages/about.md` |
| Acknowledgment entries | `_publications/2024-*-ack-*.md` |
| Portfolio items | `_portfolio/project-*.md` |
| CV | `_pages/cv.md` |
| Top navigation | `_data/navigation.yml` |

Content marked `*to be added*` is placeholder — fill in the real details.

## Run locally

```bash
bundle install
bundle exec jekyll serve --livereload
# → http://localhost:4000/HaiTang/
```

Or with the bundled Docker setup:

```bash
docker compose up
```

## Deploy

Push to `master`. GitHub Pages builds with its built-in Jekyll and serves the
site at the URL above. (Branch is `master`, **not** `main`; Pages source =
`master / (root)`, legacy build type.)

## Credits

- Template: [Academic Pages](https://github.com/academicpages/academicpages.github.io) (MIT)
- Theme base: [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) (MIT)
- Glass theme, gradient system, and content: this repo

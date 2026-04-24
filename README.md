# yveh.github.io

Personal homepage of Yuheng Zhang — built with [Hexo 8](https://hexo.io) and the [Academia](https://github.com/PhosphorW/hexo-theme-academia) theme.

- **`source` branch** — Hexo source (this branch)
- **`master` branch** — generated static site, served by GitHub Pages

## Local development

```bash
npm install
npx hexo clean
npx hexo server          # preview at http://localhost:4000
```

## Build & deploy

```bash
npx hexo clean && npx hexo generate
# `public/` now contains the static site; copy it to the master branch and push.
```

## Editing content

Each section of the homepage is a markdown post in `source/_posts/` with `academia: true` in its front matter. Posts render in reverse-chronological order by date.

| File | Section |
| --- | --- |
| `00-about.md` | About + Education |
| `01-publications.md` | Publications |
| `02-experience.md` | Research Experience |
| `03-awards.md` | Awards |
| `04-teaching.md` | Teaching |

CV PDF lives at `source/attaches/CV.pdf` and is linked from the sidebar via `themes/Academia/_config.yml` (`cv_dl.dir`).

To set an avatar, drop a square image at `themes/Academia/source/img/avatar.jpg`.

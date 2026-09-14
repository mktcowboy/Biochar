# Biochar

An Obsidian research vault on biochar science, soil applications, carbon markets, and durable CDR — published as a static site with [Quartz 4](https://quartz.jzhao.xyz/).

## Live site

https://mktcowboy.github.io/Biochar/

## Structure

- `content/` — the vault notes (edit these in Obsidian or here)
- `site/` — Quartz static-site generator and configuration
- `.github/workflows/deploy.yml` — builds and deploys to GitHub Pages on every push to `main`

## Develop locally

```bash
cd site
npm install
npx quartz build --directory ../content --serve
```

Then open http://localhost:8080.

## Updating content

Edit notes under `content/`, commit, and push to `main`. The GitHub Action rebuilds and redeploys automatically.

---

Built with [Quartz](https://quartz.jzhao.xyz/) v4.5.2 (MIT, see `site/LICENSE.txt`).

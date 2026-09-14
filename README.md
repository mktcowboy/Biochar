# Biochar

An Obsidian research vault on biochar science, soil applications, carbon markets, and durable CDR — published as a static site with [Quartz 4](https://quartz.jzhao.xyz/).

## Live site

https://mktcowboy.github.io/Biochar/

## Structure

- `content/` — the vault notes (edit these in Obsidian or here)
- `site/` — Quartz static-site generator and configuration
- `docs/github-pages-deploy.yml` — Actions workflow template (add under `.github/workflows/deploy.yml` once the `workflow` OAuth scope is available)
- Currently deployed by building Quartz and pushing the `gh-pages` branch

## Develop locally

```bash
cd site
npm install
npx quartz build --directory ../content --serve
```

Then open http://localhost:8080.

## Updating content

Edit notes under `content/`, commit, and push to `main`. Until Actions is enabled, rebuild with `cd site && npm ci && npx quartz build --directory ../content --output ../public` and republish the `gh-pages` branch.

---

Built with [Quartz](https://quartz.jzhao.xyz/) v4.5.2 (MIT, see `site/LICENSE.txt`).

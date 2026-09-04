---
layout: default
title: GitHub Pages Deployment
---

# GitHub Pages Deployment

This repository publishes the static site at:

https://cloudshare360.github.io/aws-cloud-engineer-road-map/

## Configuration

1. The repository is public and the default branch is `main`.
2. The Pages workflow builds the `docs/` source with Jekyll.
3. Jekyll converts Markdown files to `.html` pages.
4. The shared layout loads Mermaid.js for diagram code blocks.
5. The workflow uploads `_site/` as the Pages artifact.

## Deployment Steps

1. Make website changes under `docs/`.
2. Keep page links pointed at generated `.html` files, not `.md` source files.
3. Keep downloadable assets under `docs/assets/`.
4. Push to `main`, or run **Actions > Deploy to GitHub Pages > Run workflow**.
5. Confirm both `build` and `deploy` jobs succeed.

## 404 and Broken Link Checks

The deployed artifact must contain `index.html` at its top level. Run a local
Jekyll build and verify the generated routes before pushing:

```bash
jekyll build --source docs --destination _site
test -f _site/index.html
test -f _site/08-learning-roadmap-diagram.html
git diff --check
```

Project-site URLs include `/aws-cloud-engineer-road-map/`, but generated files
inside the site are addressed relative to that base path. For example:

- `/02-roadmap.html`
- `/08-learning-roadmap-diagram.html`
- `/assets/CloudEngineer-RoadMap.xlsx`

## Official References

- [GitHub Pages documentation](https://docs.github.com/en/pages)
- [Use custom workflows](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages)
- [Troubleshoot 404 errors](https://docs.github.com/en/pages/getting-started-with-github-pages/troubleshooting-404-errors-for-github-pages-sites)
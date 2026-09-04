# GitHub Pages Deployment

This repository publishes the static site from `docs/` to:

https://cloudshare360.github.io/aws-cloud-engineer-road-map/

## Configuration

1. The repository is public and the default branch is `main`.
2. `docs/index.html` is the site entry point. Its name is case-sensitive.
3. `docs/.nojekyll` disables Jekyll processing for the static HTML site.
4. GitHub Pages is configured with **Source: GitHub Actions**.
5. `.github/workflows/pages.yml` uploads the contents of `docs/` as the Pages artifact.
6. The workflow deploys that artifact to the `github-pages` environment.

## Deployment Steps

1. Make site changes under `docs/`.
2. Confirm `docs/index.html` exists at the top level of the publishing folder.
3. Push to `main`, or run **Actions > Deploy to GitHub Pages > Run workflow**.
4. Open the workflow run and confirm both `build` and `deploy` succeed.
5. Open the project URL above. Project sites include the repository name in the path.

## 404 Troubleshooting

The GitHub Pages documentation requires `index.html` at the top level of the
deployed artifact. The workflow checks this before uploading. To inspect the
artifact, download the `github-pages` artifact from a successful workflow run;
it must contain `index.html`, not `docs/index.html`.

If the artifact is correct but the URL still returns 404:

1. Confirm **Settings > Pages > Source** is **GitHub Actions**.
2. Confirm the workflow ran from `main` and the `deploy` job succeeded.
3. Check that the URL includes `/aws-cloud-engineer-road-map/`.
4. Wait briefly for Pages propagation, then retry with a cache-busting query string.
5. Check GitHub Status and the workflow deployment environment for errors.

## Local Checks

```bash
test -f docs/index.html
test ! -f docs/Index.html
git diff --check
```

## Official References

- [GitHub Pages documentation](https://docs.github.com/en/pages)
- [Configure a publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [Use custom workflows](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages)
- [Troubleshoot 404 errors](https://docs.github.com/en/pages/getting-started-with-github-pages/troubleshooting-404-errors-for-github-pages-sites)

## Continue To

- [Repository documentation index](../docs/README.md)
- [Live site](https://cloudshare360.github.io/aws-cloud-engineer-road-map/)
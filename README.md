# Deployment repository for sankalp.is-a.dev

This repository contains generated deployment output for [sankalp.is-a.dev](https://sankalp.is-a.dev). It is not the website's editable source repository.

## Source of truth

Make all code, content, and design changes in:

[`SankalpSharma7/Sankalp-comic-website`](https://github.com/SankalpSharma7/Sankalp-comic-website)

Pushing to that repository's `main` branch validates and builds the React application, then publishes `dist/` to this repository's `gh-pages` branch.

Do not edit files on `gh-pages` manually: the next successful deployment replaces them.

## Branches

- `master`: repository documentation only
- `gh-pages`: generated production files managed by GitHub Actions

Normal website releases require a push only to the source repository. Changes to this repository are needed solely for deployment-repository administration.

## Retired Jekyll website

The former Jekyll/Hank Quinlan implementation is preserved in the `legacy-jekyll-archive-2026-09-04` tag.

Publish the archive tag before merging the deployment-repository cleanup:

```bash
git push origin legacy-jekyll-archive-2026-09-04
git add .
git commit -m "Archive retired Jekyll site"
git push origin master
```

The archived files can be inspected without changing branches:

```bash
git show legacy-jekyll-archive-2026-09-04:README.md
```

# etverse

Landing site for the **etverse** — an R ecosystem for triangulating causal
evidence in epidemiology.

The site is a [Quarto](https://quarto.org) website. It states the project
philosophy (evidence / design / methodological triangulation) and links out to
each package's own documentation site at `https://etverse.github.io/<package>/`.

## Build locally

```sh
quarto preview   # live reload
quarto render    # build to docs/
```

## Deploy

This repo is intended to live at `github.com/etverse/etverse.github.io` so the
rendered site serves as the organisation landing page at
<https://etverse.github.io>. Pushing to `main` renders the site and publishes
`docs/` to the `gh-pages` branch via `.github/workflows/publish.yaml`.

## Adding a package

Edit the package grid in `index.qmd` and the design/evidence sections in
`philosophy.qmd`. Status badges: `available` (green), `in development` (amber),
`planned` (grey).

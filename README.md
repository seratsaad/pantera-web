# PANTERA — project website

Source for the PANTERA survey homepage.

**PANTERA** — Project for Astrophysical Nucleosynthesis and Targeted Exploration of
metal-Rich Abundances — is a high-resolution spectroscopic survey of the most
metal-rich stars in the solar neighborhood.

- **Live site:** https://panterasurvey.github.io  <!-- update if the org/repo name changes -->
- **Data & code (Paper I):** https://github.com/seratsaad/pantera1

## Structure

Static site, no build step.

```
index.html          # single-page site (inline CSS)
assets/
  pantera-logo.png  # wordmark
  favicon.svg       # rainbow-star favicon
  fig_cmd.png       # Gaia CMD of the 56 targets
  fig_skymap.png    # sky distribution
  fig_comp.png      # literature comparison
```

## Local preview

```
python3 -m http.server 8000   # then open http://localhost:8000
```

## Deploy

Served by GitHub Pages from the `main` branch (root). Pushing to `main` publishes.
`.nojekyll` disables Jekyll so `assets/` is served verbatim.

# Integra gateway

Minimal public recovery gateway for Integra Centros.

It checks the Cloudflare primary first and the Netlify mirror in parallel, then opens the first reachable host. The ordinary links remain available when JavaScript or the probes are unavailable.

## Hosts

- Primary: <https://integracentros.es/>
- Mirror: <https://integra-centros.netlify.app/>

If the Netlify site receives a different subdomain, update `MIRROR` and the mirror link in `index.html` before publishing.

## GitHub Pages

This repository is intentionally separate from the private application repository. Enable GitHub Pages using **GitHub Actions**; `.github/workflows/pages.yml` publishes the repository root as a static site.

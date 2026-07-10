# orthogonai.ai

Public website for **OrthogonAI** — a single self-contained `index.html`: an animated "Manhattan circuit" canvas field with one line of copy. No build step, no dependencies.

**Live:** https://orthogonai.ai/ (GitHub Pages; any push to `main` auto-deploys in ~1 min.)

## Run locally

```bash
python3 -m http.server 4179
# → http://localhost:4179
```

## Domain

Custom domain is set via the `CNAME` file (`orthogonai.ai`). DNS lives at GoDaddy: apex A records → GitHub Pages IPs, `www` CNAME → `orthogon-ai-labs.github.io`. If the domain ever changes, update `CNAME` plus the `canonical` / `og:url` / JSON-LD tags in `index.html`.

## Editing

Everything (CSS, canvas animation, favicon, JSON-LD) lives inline in `index.html`. The page is deliberately spare — one tagline, two links, the doctrine strip. Keep claims behind evidence before adding anything.

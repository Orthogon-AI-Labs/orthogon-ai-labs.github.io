# orthogon.site

Public website for **Orthogon AI Labs** — a single self-contained `index.html`, no build step, no dependencies.

## Run locally

```bash
python3 -m http.server 4179
# → http://localhost:4179
```

## Deploy (GitHub Pages, org root site)

```bash
gh repo create Orthogon-AI-Labs/orthogon-ai-labs.github.io --public --source . --push
gh api repos/Orthogon-AI-Labs/orthogon-ai-labs.github.io/pages -X POST -f 'source[branch]=main' -f 'source[path]=/'
# → https://orthogon-ai-labs.github.io
```

When a custom domain lands, add a `CNAME` file and update the `canonical` / `og:url` tags in `index.html`.

## Editing

Everything (CSS, JS, favicon, JSON-LD) lives inline in `index.html`. Content sections in order: hero → focus → systems index → approach → open source → contact. Status chips in the systems index are deliberately conservative — keep claims behind evidence.

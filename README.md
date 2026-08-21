# FPL Auto-Manager - Live Site

A public dashboard showing what my automated Fantasy Premier League
manager is currently doing - squad, captaincy, and recent transfer
decisions.

`status.json` is published automatically by the (private) automation
repo after every run - dry run, daily preview, or live - so this stays
current even on days with no actual changes.

This repo intentionally contains **no strategy logic** - no scoring
weights, no decision code, just the resulting data and a static page
that renders it. The "how" stays in the private automation repo; this
is just the "what."

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Hosting

Cloudflare Pages, auto-deployed from this repo on every push to `main`.

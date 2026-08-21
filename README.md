# FPL Auto-Manager - Live Site

A public dashboard showing what my automated Fantasy Premier League
manager is currently doing - squad, captaincy, and recent transfer
decisions.

`status.json` is published automatically by the (private) automation
repo after every run - dry run, daily preview, or live - so this stays
current even on days with no actual changes.

`strategy.html` explains the scoring model in plain English, including
the actual weights and constants - kept in sync by hand whenever the
private repo's `STRATEGY.md` changes. `changelog.json` is a manually
curated, plain-English change feed (dated from the private repo's real
commit history) - update both whenever a strategy/logic change ships.

This repo still contains **no actual code** from the private automation
repo - no Python, no file/line references, nothing runnable. It's a
description of the logic, not the logic itself.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Hosting

Cloudflare Pages, auto-deployed from this repo on every push to `main`.

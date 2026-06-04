# clawventures.llc

Static one-page site for **Claw Ventures LLC**, served via GitHub Pages at [clawventures.llc](https://clawventures.llc).

Built 2026-06-04 as the public web presence for Apple Developer Organization enrollment validation.

## Setup

| Piece | Where |
|---|---|
| Domain registration + DNS | Porkbun |
| Email | Purelymail (domain-wide catch-all — any `@clawventures.llc` address delivers) |
| Hosting | GitHub Pages, deploying from `main` branch root |
| TLS | Auto-issued by GitHub (Let's Encrypt) |

- `CNAME` pins the custom domain — **don't delete it**.
- `.nojekyll` skips the Jekyll build.

## Updating the site

Edit `index.html`, commit, push to `main`. GitHub Pages rebuilds automatically in about a minute.

## DNS records (at Porkbun)

| Type | Host | Answer |
|---|---|---|
| A | (apex) | 185.199.108.153 |
| A | (apex) | 185.199.109.153 |
| A | (apex) | 185.199.110.153 |
| A | (apex) | 185.199.111.153 |
| CNAME | www | clawv-dev.github.io |

⚠️ MX/TXT records at Porkbun belong to Purelymail (mail routing + SPF/DKIM) — never remove them.

Fuller doc: Claw Ventures Obsidian vault → `01_Notes/Domain & Website — clawventures.llc.md`.

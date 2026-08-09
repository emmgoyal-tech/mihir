# mihir-goyal.com

Personal resume site for Mihir Goyal, with the Vision for All project site nested under it.

| Page | Source | URL |
|---|---|---|
| Resume | `index.html` | https://mihir-goyal.com/ |
| Vision for All | `visionforall/index.html` | https://mihir-goyal.com/visionforall/ |

Both pages are single-file, hand-written HTML/CSS/JS — no build step. Push to `main` and GitHub Pages redeploys.

> **Note:** this repo is public. This file documents only IDs that already appear
> in the served page source. Never commit passwords, API keys, or tokens here.

## Hosting & domain

| What | Value |
|---|---|
| Hosting | GitHub Pages, repo `emmgoyal-tech/mihir`, branch `main` |
| Custom domain | `mihir-goyal.com` (via `CNAME` file) |
| DNS / registrar | *(fill in: registrar account holding mihir-goyal.com)* |

## External services

### Formspree — contact form backend (Vision for All page)

| What | Value |
|---|---|
| Purpose | Receives contact-form submissions and emails them |
| Endpoint | `https://formspree.io/f/xnpajwey` (form ID `xnpajwey`) |
| Used in | `visionforall/index.html` — `<form id="contactForm" action=…>` + fetch submit handler |
| Dashboard | https://formspree.io (Submissions tab = full history) |
| Notification email | mihir.goyal01@gmail.com |
| Limits | Free tier: 50 submissions/month |
| Set up | 2026-08-08 |

### Cusdis — "Words of Support" public message wall (Vision for All page)

| What | Value |
|---|---|
| Purpose | Moderated public comment wall — visitors post with just a name, no account |
| App ID | `a661eb12-9e31-4127-88eb-2c2bb3e3269b` |
| Page ID | `visionforall-words-of-support` (fixed — all messages land on one thread; don't change it or existing messages disappear from the page) |
| Used in | `visionforall/index.html` — `#cusdis_thread` div + `cusdis.es.js` script |
| Dashboard | https://cusdis.com — **new messages are hidden until approved here** |
| Moderation | Enable email notifications in Cusdis settings so approvals aren't missed |
| Set up | 2026-08-08 |

### Google Analytics — traffic (resume page only)

| What | Value |
|---|---|
| Measurement ID | `G-Q7GTWR8YKY` |
| Used in | `index.html` head (gtag.js) — **not** on the Vision for All page |
| Dashboard | https://analytics.google.com |

### Other references

- **Google Fonts** — Cormorant Garamond + DM Sans (resume), Nunito (Vision for All). No account; loaded from `fonts.googleapis.com`.
- **Blog** — https://goyalmihir.blogspot.com (linked from the Vision for All page and footer).
- **Footer social links** (Vision for All) — Instagram/Twitter are placeholders (`href="#"`), pending real profile URLs.

## Operational notes

- **Contact email everywhere:** `mihir.goyal01@gmail.com`.
- The Vision for All contact form falls back to Formspree's hosted page when JavaScript is off.
- ReSpectacle timeline (Vision for All) has "Photo coming soon" placeholders awaiting real photos in `visionforall/images/`.
- An old standalone repo `mihirgoyal-gc/visionforall` is **abandoned** — this repo's `visionforall/` folder is the only maintained copy.

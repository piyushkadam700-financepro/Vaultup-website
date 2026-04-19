# VaultUp — Company Website

> **vaultup.co.uk** — Professional landing page for VaultUp, the AI money coach for 16–28 year olds in the UK.

[![Live](https://img.shields.io/badge/live-vaultup.co.uk-EF9F27?style=flat-square)](https://vaultup.co.uk)
[![App](https://img.shields.io/badge/app-vaultup.vercel.app-111113?style=flat-square)](https://vaultup.vercel.app)
[![Deployed on Vercel](https://img.shields.io/badge/deployed%20on-Vercel-black?style=flat-square&logo=vercel)](https://vercel.com)

---

## Overview

This repository contains the marketing and company website for VaultUp — separate from the main app repository. The website serves as the public-facing home for VaultUp: for users discovering the product, press, investors, and professional contacts.

| URL | Purpose |
|-----|---------|
| [vaultup.co.uk](https://vaultup.co.uk) | Company website — this repo |
| [vaultup.vercel.app](https://vaultup.vercel.app) | Live app — [main repo](https://github.com/piyushkadam700-financepro/Vaultup) |

---

## About VaultUp

VaultUp is an AI-powered personal finance app built specifically for 16–28 year olds in the UK. It combines real-time AI coaching via the Anthropic Claude API, personal goal tracking, group savings with individual pot architecture, spending insights, and gamification — with a clear roadmap into Open Banking.

**67% of 18–28 year olds in the UK have no structured savings habit** (FCA Financial Lives Survey, 2022). VaultUp addresses this through personalised, data-driven coaching rather than generic advice — the AI coach (Val) has direct access to the user's income, spending categories, savings targets, and goal progress before responding to any query.

### Key numbers

- **51+ registered users** — 8 weeks live, zero paid acquisition
- **5-phase Open Banking roadmap** — FCA-aligned, regulatory pathway documented
- **Anthropic Claude API** — dynamic system prompt engineering per message
- **Supabase auth + RLS** — production-grade database with Row Level Security

---

## Tech stack

| Layer | Technology |
|-------|-----------|
| Frontend | Vanilla HTML, CSS, JavaScript — zero dependencies |
| Fonts | Bebas Neue + DM Sans via Google Fonts |
| Deployment | Vercel — auto-deploy from GitHub |
| Domain | vaultup.co.uk |

The website is intentionally a single `index.html` file — zero build pipeline, zero dependencies, instant deploy. Changes go live in under 90 seconds from commit.

---

## Repository structure

```
vaultup-website/
├── index.html      # Complete landing page — all CSS and JS inline
├── LICENSE         # Proprietary — all rights reserved
├── NOTICE          # Copyright attribution
└── README.md       # This file
```

---

## Local development

No build step required. Open `index.html` directly in any browser:

```bash
# Clone the repo
git clone https://github.com/piyushkadam700-financepro/vaultup-website.git
cd vaultup-website

# Open in browser — that's it
open index.html
```

Or serve locally with any static server:

```bash
# Using Python
python3 -m http.server 8080

# Using Node
npx serve .
```

---

## Deployment

Deployed via Vercel with automatic GitHub integration. Every push to `main` triggers a deployment.

```
Push to main → Vercel build → Live on vaultup.co.uk (~90 seconds)
```

**Domain configuration:**
- Primary domain: `vaultup.co.uk`
- DNS managed via domain registrar pointing to Vercel nameservers

---

## Related repositories

| Repo | Description |
|------|-------------|
| [Vaultup](https://github.com/piyushkadam700-financepro/Vaultup) | Main app — AI coach, goal tracking, group savings, Supabase backend |
| [vaultup-website](https://github.com/piyushkadam700-financepro/vaultup-website) | This repo — company landing page |

---

## Founder

**Piyush Kadam** — Founder & Product Builder  
ACCA Part-Qualified · MSc Accounting & Finance · Bristol, UK  

- Website: [vaultup.co.uk](https://vaultup.co.uk)
- App: [vaultup.vercel.app](https://vaultup.vercel.app)
- Contact: [hello@vaultup.app](mailto:hello@vaultup.app)

---

## License

© 2026 VaultUp. All rights reserved.  
This repository is proprietary. Unauthorised copying, modification, or distribution is prohibited.  
See [LICENSE](./LICENSE) for full terms.

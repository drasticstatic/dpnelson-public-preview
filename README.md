# Douglas P Nelson Coaching — dpnelson.com
> *Become Who You Are · Get The Right Sense of Direction*

[![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey?style=flat)](https://github.com/drasticstatic/.github)
[![Public Preview](https://img.shields.io/badge/%F0%9F%8C%90%20Public%20Preview-Available-brightgreen)](https://drasticstatic.github.io/dpnelson-public-preview/) [![Synced via GitExporter](https://img.shields.io/badge/Synced%20via-GitExporter-blue)](https://github.com/open-condo-software/gitexporter) [![Built with Claude Code](https://img.shields.io/badge/Built%20with-Claude%20Code%20CLI-blueviolet)](https://code.claude.com/docs/en/overview) [![Status](https://img.shields.io/badge/Status-%F0%9F%94%A5%20Firecrawl%20Build-orange)](https://github.com/drasticstatic/dpnelson) [![Sync](https://github.com/drasticstatic/dpnelson/actions/workflows/sync-public.yml/badge.svg)](https://github.com/drasticstatic/dpnelson/actions/workflows/sync-public.yml)

---

## Migration from Wordpress -> Vite -> next.js/Astro

**🌐 [Explore the Public Preview →](https://drasticstatic.github.io/dpnelson-public-preview/)**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**🌐 [Explore the Current Wordpress →](https://www.dpnelson.com/)**

---

> 🔒 **Public mirror notice:** This repository is partially mirrored to a public preview via an automated GitExporter pipeline. The public version includes only sanitized source files. Private configuration, credentials, setup docs, and workflow files are excluded.

---

## 👋 Hello, Douglas

**dpnelson.com** is the home of Douglas P Nelson's IFS (Internal Family Systems) coaching practice — a focused, high-performance rebuild of his existing WordPress site with absolute content fidelity and a significantly upgraded visual and motion presentation layer.

This private repo is the build workspace. The public preview (`dpnelson-public-preview`) is the filtered output automatically synced on every push to `main`.

**Primary owner:** Douglas P Nelson (`dpnelsons@gmail.com`)
**Developer / builder:** Christopher Wilson (`drasticstatic`)
**AI agents:** Alfred (Claude Code CLI) — primary frontend engineer

---

## 🎯 The Goal

Reconstruct `dpnelson.com` (currently WordPress) as a high-performance Vite + React static site with:

- **Content fidelity** — every heading, paragraph, and structural phrase from the original site preserved exactly
- **IFS coaching messaging** — resolution, clarity, parts alignment, hidden conflicts — no invented buzzwords
- **Kinetic hero section** — profile photo with ambient floating/morphing motion, staggered fade-in on load
- **Scroll-driven parallax** — Framer Motion `useScroll` + `useTransform` on major section transitions
- **Interactive Parts Alignment Interface** — multi-state UI for selecting conflicting professional emotions
- **Perspective Vault** — structured masonry layout for the "Perspective" content series
- **Frictionless intake flow** — Discovery → Clarity → Alignment → Action steps
- **Calendly widget** — book a consultation, embedded natively

---

## 🚀 Capabilities

### Core Features
- Kinetic hero section with profile photo and Framer Motion ambient animation
- Scroll-linked parallax section transitions
- Parts Alignment interactive interface (multi-state IFS coaching UI)
- Perspective Vault (masonry layout / password-protected)
- Intake Action Matrix (Discovery → Clarity → Alignment → Action)
- Calendly booking integration
- Google Apps Script form backend (saves to Drive, sends confirmation email)

### Technical
- Vite 6 + React 18 + TypeScript — SPA static build
- Tailwind CSS — utility-first, custom animation keyframes (float, morph, fadeInUp)
- Framer Motion 11 — `useScroll`, `useTransform`, `AnimatePresence`
- shadcn/ui component primitives (Radix UI + Lucide Icons)
- GitHub Pages deployment via `docs/` output dir
- Private → public sync via `sync-public.yml` GitHub Action

---

## 🏗️ Architecture

```
Private Repo (source + secrets)          Public Repo (GitHub Pages host)
github.com/drasticstatic/dpnelson  →→→  github.com/drasticstatic/dpnelson-public-preview
        │                                        │
        │  sync-public.yml (on push to main)     │
        │  builds → docs/ → pushes filtered      │
        └──────────────────────────────────────► └── GitHub Pages live URL
```

```text
src/
├── assets/              # Media files, motion SVGs, icon definitions
├── components/          # Reusable UI elements (Hero, PartsAlignment, Footer)
├── layout/              # Layout.tsx — global header, parallax container, footer
├── App.tsx              # Root render
├── index.css            # Tailwind directives + base styles
└── main.tsx             # Application mount
```

---

## 🛠️ Local Development

```bash
# Clone and install
git clone https://github.com/drasticstatic/dpnelson.git
npm ci

# Dev server (hot reload)
npm run dev
# → http://localhost:5173/dpnelson-public-preview/

# Production build (outputs to docs/)
npm run build

# Preview build locally
npm run preview
```

---

## 🚀 Deployment

Every push to `main` triggers `.github/workflows/sync-public.yml`:

1. `npm ci && npm run build` — compiles to `docs/`
2. Clones `dpnelson-public-preview` (authenticated via `PUBLIC_REPO_TOKEN` secret)
3. Copies `docs/` output to the public repo
4. Commits and pushes — GitHub Pages serves the new build automatically

**Live URL:** `https://drasticstatic.github.io/dpnelson-public-preview/`

**Custom domain (future):** Add `CNAME` file + configure DNS A-record at registrar.

---

## 🔐 Security

- All credentials, `.env` files, GWS tokens, and `service_account.json` are in `.gitignore` — never committed
- `setup/`, `scripts/`, `.github/`, `CLAUDE.md`, `AGENTS.md`, `PENDING-TASKS.md` are excluded from the public preview via `gitexporter.config.json`
- Branch protection on `main`: deletion and force-push blocked (`branch-protection/ruleset.json`)
- `*.json` files blocked by `.gitignore` except explicit exceptions (`package.json`, `tsconfig*.json`, etc.)

---

## 🌐 Related Repos

| Repo | Purpose |
|------|---------|
| [dpnelson-public-preview](https://github.com/drasticstatic/dpnelson-public-preview) | Public GitHub Pages host (filtered output) |
| [pir-devine-news](https://github.com/drasticstatic/pir-devine-news) | Pattern reference — dual-repo sync architecture |
| [wilson-lawn-assist](https://github.com/drasticstatic/wilson-lawn-assist) | Pattern reference — component templates |

---

## 📞 Contact

**Douglas P Nelson** — `dpnelsons@gmail.com` — [dpnelson.com](https://dpnelson.com)
**Developer** — Christopher Wilson — `drasticstatic@gmail.com`

---

*Built and maintained by [drasticstatic](https://github.com/drasticstatic) with Anthropic Claude Code CLI*

*🗺️ Looking for something specific? → [Public Preview](https://drasticstatic.github.io/dpnelson-public-preview/)*

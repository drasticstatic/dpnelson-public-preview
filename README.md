# 🤖 dpnelson — Douglas P Nelson

> *Become Who You Are · Get The right Sense of Direction*

[![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey?style=flat)](https://github.com/drasticstatic/.github)
[![Public Preview](https://img.shields.io/badge/%F0%9F%8C%90%20Public%20Preview-Available-brightgreen)](https://drasticstatic.github.io/dpnelson-public-preview/) [![Synced via GitExporter](https://img.shields.io/badge/Synced%20via-GitExporter-blue)](https://github.com/open-condo-software/gitexporter) [![Built with Claude Code](https://img.shields.io/badge/Built%20with-Claude%20Code%20CLI-blueviolet)](https://code.claude.com/docs/en/overview) [![NVIDIA NIM](https://img.shields.io/badge/Powered%20by-NVIDIA%20NIM-76b900)](https://build.nvidia.com/) [![Status](https://img.shields.io/badge/Status-%F0%9F%94%A5%20Live-brightgreen)](https://code.claude.com/docs/en/cli-reference) [![Sync](https://github.com/drasticstatic/dpnelson/actions/workflows/sync-public.yml/badge.svg)](https://github.com/drasticstatic/dpnelson/actions/workflows/sync-public.yml)

---

**🌐 [Explore the Public Preview →](https://drasticstatic.github.io/dpnelson-public-preview/)**

---

> 🔒 Public mirror notice: This repository is partially mirrored to a public preview via an automated GitExporter pipeline. The public version includes this README and session export files. Private configuration files, API keys, and sensitive operational notes are excluded.

> 🔒 Note for visitors: This repository is partially mirrored to a public preview via an automated GitExporter pipeline. The public version includes this README and session export files. Private configuration files, API keys, and sensitive operational notes are excluded.

---

## 👋 Hello, ...

**platform:**

---

## 🎯

**The Goal:**

---

## 🚀 Capabilities

### Core

### Technical

---

## Integration

### Launch

---

## 📁 My Workspace

```
```

### Key Files

---

## 🤝 

---

## 🏗️ Architecture

---

## 🔐 Security

---

## 🌐 Related Repos

---

## 📞 Contact

---

# dpnelson.com — Internal Family Systems (IFS) Coaching Platform

A modern, high-performance reconstruction of the official website for Douglas P. Nelson's international coaching practice. Built using a streamlined static React architecture, this iteration preserves absolute content fidelity while upgrading visual presentation layers with dynamic animation primitives and smooth scroll-linked motion effects.

## 🏗️ Technical Stack

- **Framework Core:** [Vite](https://vitejs.dev) + [React](https://react.dev) (Single Page Application architecture)
- **Styling Pipeline:** [Tailwind CSS](https://tailwindcss.com) (Utility-first configuration)
- **Component Primitives:** [shadcn/ui](https://shadcn.com) (Radix UI + Lucide Icons)
- **Animation System:** [Framer Motion](https://framer.com) (Parallax hooks & kinetic containers)

---

## 🛠️ Local Development Setup

Follow these steps to initialize, configure, and execute the workspace environment locally using your preferred package manager and development workflow.

### 1. Clone & Install Dependencies
Ensure you have [Node.js (v20+)](https://nodejs.org) installed on your machine.
```bash
# Clone the repository
git clone github.com

# Install clean node modules
npm ci
```

### 2. Configure Tailwind CSS Primitives
Initialize the styling workspace if running fresh setups:
```bash
npx tailwindcss init -p
```

### 3. Run Local Server
Spin up the Vite development server to test page transformations, state changes, and animation timing in real time.
```bash
npm run dev
```
Open your browser and navigate to `http://localhost:****`.

---

## 📦 Project Architecture

```text
└── src/
    ├── assets/              # Media files, motion SVGs, and icon definitions
    ├── components/          # Reusable UI elements (Hero, Interactive Parts, Footer)
    ├── layout/              # Structural wrappers and global parallax containers
    ├── App.tsx              # Main page scaffolding and content mapping
    ├── index.css            # Tailwind directives and baseline CSS rules
    └── main.tsx             # Application mount layer
```

---

## 🚀 Deployment Infrastructure

This pipeline utilizes a dual-stage deployment architecture to handle client staging reviews separately from the live production site.

### 👥 1. Staging & Client Previews (Automated)
Every code check-in pushed triggers a background GitHub Actions runner. This automatically bundles the production directory and pushes the built artifacts to the `gh-pages`

### 🔒 2. Final Production Handover
Once design updates are signed off by the client, the code is ready for live hosting infrastructure (Netlify, Vercel, or Cloudflare Pages) with absolute zero runtime footprint.

```bash
# Compile and optimize production distribution package
npm run build
```
The resulting optimized static payload will generate completely inside the `/dist` folder, ready to tie directly into Douglas's target production domain configuration.

---

*Built and maintained by [drasticstatic](https://github.com/drasticstatic) · w/ Anthropic's ClaudeCodeCLI + NVIDIA NIM

*🗺️ Still feeling lost? Looking for something specific? 🧭 → Click [HERE](https://drasticstatic.github.io/dpnelson-public-preview/404.html) 🔍*

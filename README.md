# QuickAI — AI-Powered SaaS Platform 

[![Release](https://img.shields.io/badge/release-v1.0.0-blue)](https://github.com/anjalihks/QuickAI/releases)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Made with MERN](https://img.shields.io/badge/stack-PERN-yellowgreen)](#tech-stack)

> QuickAI is an AI-powered SaaS platform built with the MERN stack that helps users create content and images, and refine professional assets. Create blog posts and titles, generate and edit images (background removal, object removal), and get structured resume reviews — all from a single polished web app.

---

## Demo
- **Live demo:** _(quick-ai-iota-one.vercel.app)_  

---

## Key Features

- ✍️ **Write Article** — AI-assisted long-form article generation and editor with versioning and export (Markdown / HTML).
- 🧠 **Blog Title Generator** — Instant, SEO-friendly title suggestions based on topic, tone, and keywords.
- 🖼️ **Generate Images** — Create images from prompts (supports multiple styles, aspect ratios).
- ✂️ **Remove Background** — Automatic background removal for uploaded images.
- 🪄 **Remove Object** — Intelligent object removal / inpainting in images.
- 📝 **Resume Review** — AI-driven resume analysis with section-by-section suggestions and score.
- 🔐 **Authentication & Profiles** — Secure user accounts, roles (user/admin), and usage quotas.
- ⚙️ **Admin Dashboard** — Monitor usage, manage users, view logs and billing overview.
- 🔁 **Integration Ready** — Webhooks and REST API endpoints for automation and integrations.

---

## Tech Stack

- **Frontend:** React (Vite), Tailwind CSS / Shadcn UI
- **Backend:** Node.js + Express
- **Database:** PostgreSQL (Neon)
- **Auth:** JWT / BetterAuth (or your preferred provider)
- **Background Jobs / Workflows:** Inngest / BullMQ / Redis (for async tasks)
- **AI / Vision:** OpenAI, Gemini, or other LLM & image APIs (replaceable)
- **Image Processing:** Sharp / remove.bg-style models or local ML inference
- **Deployment:** Vercel / Netlify (frontend), Vercel / Heroku / DigitalOcean (API), Neon
- **Monitoring:** Sentry / Logflare / Prometheus (optional)

---

## Quickstart — Local Development

> Prerequisites: Node.js (18+), npm or pnpm, MongoDB (local or Atlas), Redis (if using job queue)

```bash
# 1. Clone
git clone https://github.com/anjalihks/QuickAI.git
cd QuickAI

# 2. Install dependencies (run in root, frontend, and backend if separated)
npm install

# 3 Run in development
npm run dev
# or if monorepo:
# cd backend && npm run server
# cd frontend && npm run dev

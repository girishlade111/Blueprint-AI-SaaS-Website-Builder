# Blueprint: SaaS AI Website Builder

An interactive, single-page technical blueprint dashboard for an AI-powered SaaS website builder. Presented as a dark "Cosmic Night" dashboard, it walks through every pillar of the product plan — competitive analysis, AI generation pipeline, database schema, go-to-market strategy, and project scaffolding — with interactive charts, diagrams, and AI-assisted planning widgets.

## Features

- **Interactive dashboard layout** — sticky top navigation jumps between blueprint pillars (AI Core, Architecture, Competitive Analysis, Database Schema, Go-to-Market, Scaffolding) for fast reference-style exploration.
- **Competitive analysis radar chart** — Chart.js radar visualization comparing website-builder platforms across quantitative dimensions, with hover tooltips.
- **Generation pipeline flowchart** — click-to-expand HTML/CSS flowchart showing the AI generation pipeline's sequence and dependencies, with details in a modal.
- **Interactive database schema diagram** — click on a data model to view its Prisma code in a modal, with an AI-powered explanation (Gemini API).
- **Go-to-market generator** — enter a target audience and generate strategic GTM ideas via the Gemini API.
- **Project scaffolding assistant** — describe a project and get AI-suggested data models and API endpoints.
- **Dark, high-contrast theme** — deep slate background with sky-blue/teal accents (Inter font, Tailwind CSS).

## Tech Stack

- Plain HTML/CSS/JavaScript (single `index.html`, no build step)
- Tailwind CSS via CDN
- Chart.js via CDN
- Google Fonts (Inter)
- Gemini API (optional — powers the AI explanation/generator widgets)

## Quick Start

No build or dependencies required — just open the page:

```bash
git clone https://github.com/girishlade111/Blueprint-AI-SaaS-Website-Builder.git
cd Blueprint-AI-SaaS-Website-Builder
# open index.html in any modern browser
```

Or serve it locally:

```bash
npx serve .
# then visit the printed URL
```

### Gemini API (optional)

The "AI explanation" and "generator" widgets call the Gemini API. To enable them, open `index.html` and add your API key where indicated in the script (search for `GEMINI_API` / `API_KEY`). Without a key the rest of the dashboard still works.

## Project Structure

```
.
├── index.html   # The entire app: layout, styles, JS, Chart.js + Tailwind via CDN
└── README.md
```

## Deploy Notes

Static site — deploy anywhere static hosting works:

- **GitHub Pages:** enable Pages on the `main` branch (path `/`) → `https://girishlade111.github.io/Blueprint-AI-SaaS-Website-Builder/`
- **Netlify / Cloudflare Pages / Vercel:** drop the repo in; no build command needed, publish directory is the repo root.

No environment variables required (Gemini key is client-side and optional).

---

Built by Girish Lade — https://ladestack.in

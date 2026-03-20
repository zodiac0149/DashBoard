# 🎓 CapstoneIntel

> An interactive capstone project portfolio with AI-powered project exploration and an AI chatbot assistant.

## Live Demo

Deploy via [GitHub Pages](https://pages.github.com/) — see **Deployment** below.

## Features

- 📊 **Portfolio Analytics** — Doughnut & radar charts showing difficulty and domain distribution
- 🏆 **Top 3 Recommendations** — Curated advisor picks highlighted separately  
- 🔍 **Interactive Project Explorer** — Filter by difficulty, click through to full detail pages
- 🤖 **AI Chat Assistant** — Per-project Groq/Llama 3 chatbot pre-loaded with project context
- ✨ **Add Your Own Projects** — AI rewrites a rough description into a fully structured entry

## Pages

| File | Purpose |
|---|---|
| `INDEX.HTML` | Main portfolio explorer |
| `project.html` | Project detail page (driven by `?id=` URL param) |
| `add-project.html` | AI-powered project submission form |

## AI Setup (Groq — Free)

1. Get a free API key at [console.groq.com/keys](https://console.groq.com/keys)
2. Open any project detail page → click the 🤖 button → paste your key → Save
3. The key is stored **only in your browser's localStorage** — it is never in the source code

> ✅ Safe to fork/clone — no secrets in this repo.

## Adding Custom Projects

Click **✨ Add Project** in the navbar → describe your idea → the AI generates all structured fields → preview → add to portfolio.  
Custom projects are stored in `localStorage` and persist across sessions in the same browser.

## Deployment (GitHub Pages)

1. Push this repo to GitHub
2. Go to **Settings → Pages → Source → main branch → / (root)**
3. Your site will be live at `https://<your-username>.github.io/<repo-name>/`

## Tech Stack

- Vanilla HTML + CSS + JavaScript (no build step)
- [Tailwind CSS](https://tailwindcss.com/) via CDN
- [Chart.js](https://www.chartjs.org/) via CDN
- [Groq API](https://groq.com/) — Llama 3.3 70B for AI features

## License

MIT

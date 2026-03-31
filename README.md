# Vertex Capital — VC Portal

A full-stack investment management portal built with Next.js 14 + Claude AI.

## Features
- **Dashboard** — KPIs, pipeline overview, deal scoring, activity feed
- **Pipeline** — Filterable & sortable deal list with detail panel
- **Portfolio** — Portfolio companies with MOIC, IRR tracking
- **Due Diligence** — Interactive DD checklists with progress tracking
- **Term Sheet** — Clause-by-clause negotiation tracker + closing checklist
- **Analytics** — Deal funnel, sector analysis, startup metrics
- **Team Workspace** — Tasks, workflow, workload, comments, roles, notifications
- **AI Assistant** — Live Claude Sonnet integration for memos, emails, analysis

## Deploy on Render

### Step 1 — Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit — VC Portal"
git remote add origin https://github.com/YOUR_USERNAME/vc-portal.git
git push -u origin main
```

### Step 2 — Create Render Web Service
1. Go to [render.com](https://render.com) → New → **Web Service**
2. Connect your GitHub repo
3. Configure:
   - **Build Command:** `npm install && npm run build`
   - **Start Command:** `npm start`
   - **Node Version:** 18+

### Step 3 — Add Environment Variable
In Render Dashboard → Environment:
```
ANTHROPIC_API_KEY = your_api_key_here
```

Get your API key from [console.anthropic.com](https://console.anthropic.com)

### Step 4 — Deploy
Click **Deploy** — your portal will be live in ~3 minutes!

## Local Development
```bash
npm install
cp .env.example .env.local
# Add your ANTHROPIC_API_KEY to .env.local
npm run dev
# Open http://localhost:3000
```

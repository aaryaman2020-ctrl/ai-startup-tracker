# AI Startup Tracker 🌍

A comprehensive tool for tracking early-stage AI startups globally — from Pre-Seed to Series A.

## What's Inside

- **205+ companies** across **7 global regions**: North America, Europe, Asia-Pacific, India & South Asia, Middle East, Africa, Latin America
- **Live dashboard** with interactive charts, searchable directory, and world map
- **Fintech focus** tab for AI + payments/finance/e-commerce companies
- **23 startup ideas** at the intersection of AI and fintech/payments
- **Auto-updating** — new companies added weekly via automated scans

## Live Dashboard

Open `index.html` in your browser, or deploy to any static hosting (GitHub Pages, Netlify, Vercel, S3).

### Dashboard Tabs

| Tab | Description |
|-----|-------------|
| **Overview** | Key metrics, world map, stage/vertical/region charts |
| **Company Directory** | Searchable, filterable, sortable table of all companies |
| **World Map** | Companies grouped by region with expandable cards |
| **Verticals** | Companies grouped by sector/vertical |
| **Startup Ideas** | 23 curated ideas for AI + fintech founders |
| **Fintech Focus** | Companies in payments, lending, insurance, accounting |

## Data

| File | Description |
|------|-------------|
| `data/global_ai_startups.json` | Master dataset — 205+ companies with full details |
| `data/ai_startup_ideas.json` | 23 startup ideas for AI + fintech/payments |
| `data/successful_ai_startups.json` | 57 successful AI companies for reference |
| `data/success_patterns.md` | Analysis of 7 key success patterns |
| `data/emerging_verticals.md` | Vertical opportunity matrix and gap analysis |
| `data/ai_market_trends.md` | Funding trends, market data, failure patterns |

## Dataset Schema

Each company in `global_ai_startups.json` includes:

```json
{
  "company_name": "Company Name",
  "founded_year": 2024,
  "description": "What they do",
  "vertical": "Fintech / Payments",
  "stage": "Seed",
  "funding_raised": "$5M Seed (Investor Names)",
  "key_founders": "Founder Name (background)",
  "website": "https://company.com",
  "unique_value": "What makes them special",
  "location": "City, Country",
  "region": "North America",
  "date_added": "2026-03-02"
}
```

## Region Coverage

| Region | Companies |
|--------|-----------|
| North America | 91 |
| Europe | 39 |
| Asia-Pacific | 25 |
| India & South Asia | 23 |
| Africa | 10 |
| Middle East | 9 |
| Latin America | 8 |

## Stage Distribution

| Stage | Count |
|-------|-------|
| Seed | 122 |
| Series A | 44 |
| Pre-Seed | 39 |

## Built With

- Pure HTML/CSS/JS (no build step)
- [Chart.js](https://www.chartjs.org/) for data visualization
- [Inter](https://rsms.me/inter/) typeface

## License

MIT

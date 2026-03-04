# AI Startup Tracker

A comprehensive intelligence dashboard tracking **205 AI startups** across **7 regions** with **21 data fields** per company — including deep product intelligence, competitive landscapes, and investor data.

![Dashboard Preview](https://img.shields.io/badge/Companies-205-818cf8?style=flat-square) ![Regions](https://img.shields.io/badge/Regions-7-60a5fa?style=flat-square) ![Fields](https://img.shields.io/badge/Fields_per_Company-21-4ade80?style=flat-square) ![Updated](https://img.shields.io/badge/Updated-March_2026-fbbf24?style=flat-square)

## What is this?

An interactive, self-updating dashboard that tracks early-stage AI companies globally. Built for founders, investors, and researchers who want to understand:

- **What's being built** — product names, descriptions, and technical approaches
- **Who's buying** — target customers and business models
- **Who's competing** — competitive landscapes per company
- **Who's funding** — investors and funding rounds
- **Where it's happening** — geographic distribution across 7 regions

## Dataset Stats

| Metric | Value |
|--------|-------|
| Total Companies | 205 |
| Regions | 7 (North America, Europe, Asia-Pacific, India & South Asia, Africa, Middle East, Latin America) |
| Funding Stages | Pre-Seed (39), Seed (122), Series A (44) |
| Verticals | 200+ unique categories |
| Fields per Company | 21 |
| Data Files | 5 (companies, successful exits, startup ideas, success patterns, emerging verticals) |

### Regional Breakdown

| Region | Companies |
|--------|-----------|
| North America | 91 |
| Europe | 39 |
| Asia-Pacific | 25 |
| India & South Asia | 23 |
| Africa | 10 |
| Middle East | 9 |
| Latin America | 8 |

## Product Intelligence (NEW)

The dataset now includes **8 enriched product intelligence fields** for every company:

| Field | Description |
|-------|-------------|
| `product_name` | The actual product/platform name |
| `product_description` | What the product does in detail |
| `how_it_works` | Technical approach and architecture |
| `target_customer` | Who buys this product (industry, size, persona) |
| `business_model` | SaaS, usage-based, marketplace, API, etc. |
| `key_differentiator` | What makes this product unique vs. alternatives |
| `competitors` | Named competitors in the same space |
| `investors` | Known investors and funding sources |

The dashboard includes a dedicated **Product Intel** tab that lets you:
- Search across all product intelligence fields
- Filter by target customer type (Enterprise, SMB, Developer, etc.)
- Filter by business model (SaaS, API, Usage-based, etc.)
- Click any company card to open a full detail modal with all 21 fields

## Data Schema

Each company record contains these 21 fields:

```json
{
  "company_name": "string",
  "founded_year": "number",
  "description": "string",
  "vertical": "string",
  "stage": "string (Pre-Seed | Seed | Series A)",
  "funding_raised": "string",
  "key_founders": "string",
  "website": "string (URL)",
  "unique_value": "string",
  "location": "string",
  "region": "string",
  "source": "string",
  "date_added": "string (YYYY-MM-DD)",
  "product_name": "string",
  "product_description": "string",
  "how_it_works": "string",
  "target_customer": "string",
  "business_model": "string",
  "key_differentiator": "string",
  "competitors": "string",
  "investors": "string"
}
```

## Dashboard Tabs

| Tab | Purpose |
|-----|---------|
| **Overview** | KPI cards, global map, stage/region/vertical/year charts |
| **Directory** | Searchable, sortable, paginated table of all 205 companies. Click any row to open full detail modal |
| **Product Intel** | Browse companies by product intelligence — target customer, business model, competitors. Filter and search across all enriched fields |
| **World Map** | Region cards with expandable company lists grouped by vertical |
| **Verticals** | All 200+ verticals as collapsible sections with company cards |
| **Startup Ideas** | 23 vetted AI startup opportunities with market sizing and moat analysis |
| **Fintech Focus** | AI companies in financial services (payments, lending, insurance, etc.) |

## How to Use

### Option 1: GitHub Pages
1. Enable GitHub Pages in Settings → Pages → Source: `main` branch
2. Visit `https://yourusername.github.io/ai-startup-tracker/`

### Option 2: Local Server
```bash
cd ai-startup-tracker
python3 -m http.server 8000
# Open http://localhost:8000
```

> **Note:** The `index.html` loads data via `fetch()` from the `data/` folder, so it requires a web server. Opening the file directly in a browser will not work due to CORS restrictions.

## File Structure

```
├── index.html                          # Dashboard (fetch-based, for web server / GitHub Pages)
├── data/
│   ├── global_ai_startups.json         # 205 companies × 21 fields (main dataset)
│   ├── successful_ai_startups.json     # Successful AI company case studies
│   ├── ai_startup_ideas.json           # 23 vetted startup opportunities
│   ├── success_patterns.md             # Analysis of AI startup success patterns
│   └── emerging_verticals.md           # Emerging AI vertical analysis
└── README.md
```

## Auto-Update

The dataset is refreshed weekly with automated scans that:
- Discover new AI startups across all 7 regions
- Enrich existing companies with updated funding, product, and competitive data
- Add new verticals as they emerge
- Update investor and competitor landscapes

## License

This dataset is provided for research and educational purposes. Company data is sourced from public information.

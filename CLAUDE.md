# Mayaro Beach Houses - Claude Instructions

## Project Overview
Online booking agency SPA for beach house rentals in Mayaro, Trinidad.
Live site: https://beachhousesinmayaro.com

## Business Context
Building a full OTA (Online Travel Agency) using a phased approach toward full automation and a real estate private demand index powered by data analytics.

## Roadmap

| Phase | Stack | Pricing |
|---|---|---|
| 1. MVP | n8n + Google Sheets | Manual |
| 2. Hybrid | Postgres + Admin Dashboard | Manual |
| 3. Semi-auto | Pricing engine + holds + payment webhooks | Semi-auto |
| 4. Full auto | Host portal + automated policies + BI dashboards | Automated |

Long-term goal: single source of truth, fully automated system with BI dashboards for a real estate private demand index.

## Project Structure
- `index.html` - Main SPA (Homepage, About, Contact sections)
- `blog.html` - Separate blog page
- `assets/` - Static assets (images, CSS, JS)
- `forms/` - Backend form/booking handlers
- `robots.txt` - Search engine crawl rules
- `sitemap.xml` - Site map for SEO
- `package.json` - Dev dependencies (live-server)

## Tech Stack (Current - Phase 1)
- Static HTML/CSS/JS SPA (no framework)
- n8n for workflow automation
- Google Sheets as backend/database
- `live-server` for local development (`npm start`)
- Booking flow: user submits name, email, check-in, check-out, guests -> backend emails payment link + room images

## Development Rules
- Always assist with the current phase in mind, while keeping future phases in view
- Do not add frameworks or build tools unless required by the roadmap
- Keep changes minimal and focused
- Always provide code snippets of the actual changes made after each prompt
- Always reference code locations using clickable hyperlinks in the format [filename.ext:LINE](filename.ext#LLINE) e.g. [index.html:127](index.html#L127)
- Do not auto-commit — always ask before committing
- Do not push to remote unless explicitly asked

## SEO / Deployment Notes
- `robots.txt` blocks `/search/` directory
- `sitemap.xml` is maintained for proper indexing

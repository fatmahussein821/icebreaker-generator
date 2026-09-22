#  Icebreaker Generator

An **n8n lead-research and personalization pipeline** designed to discover prospects in any selected location, enrich company information, and generate formal, automation-focused email icebreakers with AI.

## What it does

- Runs on a scheduled basis and launches an Apify lead-scraping actor.
- Discovers prospects based on the selected location and search criteria.
- Filters leads that contain an email address, phone number, and company domain.
- Fetches company websites and extracts useful links.
- Uses Gemini to select the most relevant company pages without unnecessary browsing.
- Normalizes and limits the selected links before fetching their content.
- Generates a professional icebreaker connected to automation, operational efficiency, reporting, and workflow optimization.
- Aggregates the enriched lead data for downstream storage in Google Sheets.

## Workflow architecture

`Schedule → Scrape UAE leads → Filter → Format lead → Fetch website → Extract links → Select relevant URLs with Gemini → Normalize → Fetch selected pages → Generate icebreaker → Aggregate → Google Sheets`

## Integrations

- n8n
- Apify
- Google Gemini
- Google Sheets
- JavaScript normalization and validation


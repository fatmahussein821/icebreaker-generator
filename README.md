# Project Managers UAE – Icebreaker Generator

An **n8n lead-research and personalization pipeline** designed to discover project managers in the United Arab Emirates, enrich company information, and generate formal, automation-focused email icebreakers with AI.

## What it does

- Runs on a scheduled basis and launches an Apify lead-scraping actor.
- Filters leads that contain an email, phone number, and company domain.
- Fetches company websites and extracts useful links.
- Uses Gemini to select the most relevant company pages without unnecessary browsing.
- Normalizes and limits selected links before fetching their content.
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

## Setup

1. Import `ProjectManagersUAE-IcebreakerGenerator.json` into n8n.
2. Configure Apify and Google Gemini credentials.
3. Configure the Google Sheets destination and any webhook settings.
4. Review the prompt and lead filters for the target audience.
5. Test with a small result count before enabling the schedule.

Credentials and instance identifiers are represented by placeholders in the exported workflow.

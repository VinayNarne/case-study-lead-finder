# Case study: lead research tool for an electrical contractor

This repo is a write-up only. The code and data are not included.

## The problem

When a technician arrives at a job site, the team wants to know which nearby businesses might need electrical work, so they can make a warm call.

## What it does

Enter a job address. The tool collects nearby businesses from 14 data sources, removes duplicates, filters by company size and writes a short sales brief with an opening line for each lead. It takes about 8 to 12 seconds for 5 leads. A scheduled scan emails a digest of new permits.

## Architecture

- Python and FastAPI, deployed on Railway.
- Public and open-data sources such as Google Places, OpenStreetMap and Ontario city open data.
- Azure OpenAI writes the briefs. The opening line is a fixed template so the call script stays consistent.
- SQLite for local business data.

## How I worked

I designed the system and wrote it with AI coding assistants, then tested and deployed it.

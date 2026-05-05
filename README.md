# Open Government Data API

I built this API to make government data easier to access and work with. Instead of scraping multiple websites or digging through PDFs, you can just query this API and get clean data back.

**Live here:** [(https://8a0b289c-7312-47c2-80d8-340b1d1d3c0e-00-3ivh3jvapmlg7.janeway.replit.dev/docs)]

## What this does

Basically, I took several CSV files (organizations, resources, user records, tags) and loaded them into a PostgreSQL database. Then I built a simple API on top so you can filter, search, and pull whatever data you need.

Right now you can:
- Get all available datasets
- Filter by organization or tags
- Search across the data
- See which government bodies published what

## How I built it

- **Python** with Flask (simple, gets the job done)
- **PostgreSQL** for the database
- **Render** to host it (so it's actually live)
- **Pandas** to clean the CSVs before loading

The files in this repo:
- `mainf.py` – the actual API code
- `dump.sql` – database schema + data
- `requirements.txt` – what you need to install
- `erd_milestone1.png` – database diagram (visual)
- `/data` – the original CSVs

## Run it yourself

If you want to try it locally:

```bash
git clone https://github.com/SalmaSameeh/open-government-data-api.git
cd open-government-data-api
pip install -r requirements.txt
python mainf.py

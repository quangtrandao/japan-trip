# Japan Trip Map (Osaka → Tokyo)

Interactive Leaflet map of a 13-day Japan itinerary, generated from the Notion
database **"Hokuriku 2 – November 2027"**.

## Structure

- `src/index.html` — the interactive map (Leaflet + OpenStreetMap/CARTO/GSI tiles)
- `src/img/` — photos for each stop and day trip

## Updating

1. Edit the trip in the Notion database.
2. Regenerate `src/index.html` from Notion (or ask OpenCode to do it).
3. Commit and push — Vercel redeploys automatically.

## Deploy

Served by the Vercel project `japan-trip-map`, from the `src/` directory.

## Deploy verification

Pipeline test: push to `main` → Vercel auto-deploy (verified 2026-10-08).

## Notes

- Day-trip photos and stop photos are referenced as `img/*.jpg`.
- The CARTO API key is embedded in the page source; keep the site private or
  restrict the key by domain in the CARTO dashboard.

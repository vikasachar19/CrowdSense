# CrowdSense

Smart crowd monitoring dashboard — single-page web app for tracking live crowd density, alerts, and routes across multiple venues.

## Features

- **Live venue map** (Leaflet) with zone-based crowd density overlays and colored routes
- **Multi-venue switching**, including preset locations like Kempegowda International Airport
- **Search** with local place matching + Nominatim (OpenStreetMap) fallback for arbitrary locations
- **Visitor traffic chart** (Chart.js) with historical/peak tracking
- **Alerts feed**, route status panel, and zone table
- **Weather widget** with °C/°F toggle
- **Simulation mode** for demo/testing crowd data over time
- **Compass + bearing** calculations for route orientation

## Tech stack

- Vanilla JS, HTML, CSS — no build step, single file
- [Leaflet.js](https://leafletjs.com/) v1.9.4 — mapping
- [Chart.js](https://www.chartjs.org/) v4.4.0 — visitor traffic charts
- [Nominatim](https://nominatim.org/) (OpenStreetMap) — geocoding search

## Running locally

Just open the HTML file in a browser — no build/install needed:

```bash
open CrowdSense_1_5_2.html
```

Or serve it locally if you hit CORS issues with the Nominatim API:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000/CrowdSense_1_5_2.html
```

## Status

Version 1.5.2 — actively evolving. Current data is simulated/static, not connected to a live crowd-sensing backend.

## Notes

Built with AI-assisted development (Claude).

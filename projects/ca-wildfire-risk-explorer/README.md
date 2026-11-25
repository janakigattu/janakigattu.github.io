# California Wildfire Risk Explorer

Your land decision is only as good as the risk picture behind it. This app puts the two layers that matter on one map, in thirty seconds, with no sign-up and no software to install: CAL FIRE Fire Hazard Severity Zones and current wildfire activity from ArcGIS Living Atlas.

## What it does

- Shows the adopted CAL FIRE Fire Hazard Severity Zones (effective April 1, 2024) as a live ArcGIS REST layer, with Moderate, High, and Very High hazard classes.
- Shows current USA wildfire activity from ArcGIS Living Atlas, so hazard and live fire are never confused with each other.
- Lets you switch between topographic and imagery basemaps, and toggle each data layer on and off.
- Click anywhere on the map to identify the hazard zone at that point.
- Explains, in plain language, what the zones mean, what the live layer shows, and what the map does not do.

## How to run it

Open `index.html` in a browser, or serve the folder with any static server. The app needs internet access: Leaflet and Esri Leaflet load from the unpkg CDN, and the data layers load live from Esri's public ArcGIS REST services. No API key, no account, no build step.

## Data sources

- CAL FIRE Fire Hazard Severity Zones, adopted April 1, 2024 (layer 0, class field `FHSZ_Descr`): `https://services.arcgis.com/12ZpLdNBJek66bmF/arcgis/rest/services/FHSZ_SRA24_LRA25_CF_Local_Merge_20251208/FeatureServer/0`
- USA Wildfires, past 7 days (ArcGIS Living Atlas; layer 0 current incidents, layer 1 current perimeters): `https://services1.arcgis.com/P946On66WOQ606jN/arcgis/rest/services/USA_Wildfires_JF/FeatureServer`
- Basemaps: Esri World Topo and World Imagery tile services.

## Before publishing

All three layer URLs were verified live on 2026-11-24 (the first draft used two service addresses that return 400 "Invalid URL" — those services moved — and were replaced with the verified ones above). Before this app goes live on GitHub Pages, open it in a browser and confirm the layers draw and the layer-status panel reports "loaded" for each. The app reports a failed layer in its status panel rather than failing silently.

## Limits

- Hazard zones are a planning input, not a parcel-level verdict.
- This is not an evacuation or emergency map. For live evacuation orders and current incidents, use CAL FIRE and your county emergency site.
- Live fire data depends on reporting and can lag a new start.

## Built by

Janaki Gattu, Enterprise GIS Consultant & GIS Solutions Architect — [janakigattu.github.io](https://janakigattu.github.io) · [github.com/janakigattu](https://github.com/janakigattu) · [LinkedIn](https://www.linkedin.com/in/janaki-gis-enterprise)

## Call to action

If your organisation makes land, planning, or infrastructure decisions in fire country and needs a hazard tool built on your own data, get in touch: [gjanaki360@gmail.com](mailto:gjanaki360@gmail.com?subject=Wildfire%20and%20hazard%20GIS%20help) — or book a session from the portfolio home page.

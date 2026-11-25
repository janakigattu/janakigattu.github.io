# Sacramento Housing & Transit Access Explorer

A home is not just a price and a floor plan. It is a commute, a bus fare, and a walk in the rain. This app puts housing and transit on the same map for Sacramento, CA, so you can judge transit access before you judge the address, in thirty seconds, with no sign-up and no software to install.

## What it does

- Shows apartment complex locations from Sacramento County open data as a live ArcGIS REST layer.
- Shows every transit stop in the Caltrans GTFS feed, so bus and light rail stops are visible together with housing.
- Shows SacRT light rail lines (Gold, Blue, Green) and stations from SACOG's Regional Transit Network Plan.
- Lets you switch between topographic and imagery basemaps, and toggle each data layer on and off.
- Click anywhere on the map to get a plain-language answer: the apartment complex at that spot, how many transit stops sit within a five-minute walk (400 m), the nearest stop with its agency and route count, and the nearest light rail station with its distance.
- Explains, in plain language, what transit access means for a housing decision, and what the map does not do.

## How to run it

Open `index.html` in a browser, or serve the folder with any static server. The app needs internet access: Leaflet and Esri Leaflet load from the unpkg CDN, and the data layers load live from public ArcGIS REST services. No API key, no account, no build step.

## Data sources

All four service URLs were verified live on 2026-11-24 with a `?f=json` check before the app was built.

- Apartments, Sacramento County open data (layer 0, polygon; name field `LANDMARK`, description field `DESCRIPTION`): `https://services1.arcgis.com/5NARefyPVtAeuJPU/ArcGIS/rest/services/Apartments/FeatureServer/0`
- California Transit Stops, Caltrans GTFS feed via California Open Data (layer 0, point; fields `stop_name`, `agency`, `n_routes`, `route_ids_served`, `route_type`; data last updated November 19, 2025): `https://caltrans-gis.dot.ca.gov/arcgis/rest/services/CHrailroad/CA_Transit_Stops/FeatureServer/0`
- Light Rail Stations, SACOG Regional Transit Network Plan (layer 60, point; name field `STOP_NAME`): `https://services9.arcgis.com/eNX73FDxjlKFtCtH/ArcGIS/rest/services/Regional_Transit_Network_WFL/FeatureServer/60`
- Light Rail lines, SACOG Regional Transit Network Plan (layer 63, polyline; fields `short_name` with values Green, Blue, Gold, and `long_name`): `https://services9.arcgis.com/eNX73FDxjlKFtCtH/ArcGIS/rest/services/Regional_Transit_Network_WFL/FeatureServer/63`
- Basemaps: Esri World Topo and World Imagery tile services.

## Before publishing

All four layer URLs were verified live on 2026-11-24 (service JSON, layer lists, and popup fields confirmed). Before this app goes live on GitHub Pages, open it in a browser and confirm the layers draw and the layer-status panel reports "loaded" for each. The app reports a failed layer in its status panel rather than failing silently.

## Limits

- This is not a listings site. It shows where apartment complexes are, not which units are available or what they cost.
- A stop on the map is not a promise of frequent service. Check the route timetable before relying on a stop.
- Transit data is schedule data, not real time. Delays do not show up here.
- Walking distance is measured as the crow flies, not along streets. A stop 400 metres away across a freeway is not a five-minute walk.
- The transit stops layer is statewide; it only loads stops for the area on screen, so panning a long way out takes a moment to refill.

## Built by

Janaki Gattu, Enterprise GIS Consultant & GIS Solutions Architect — [janakigattu.github.io](https://janakigattu.github.io) · [github.com/janakigattu](https://github.com/janakigattu) · [LinkedIn](https://www.linkedin.com/in/janaki-gis-enterprise)

## Call to action

If your organisation makes housing, planning, or transit decisions in the Sacramento region and needs an access tool built on your own data, get in touch: [gjanaki360@gmail.com](mailto:gjanaki360@gmail.com?subject=Housing%20and%20transit%20GIS%20help) — or book a session from the portfolio home page.

# ArcGIS Online Credit Estimator

Most ArcGIS Online bills are a surprise because nobody added up the credits first. This estimator adds up the month before you spend it.

## What it does

A working estimator for ArcGIS Online credits. Enter your monthly storage (hosted features, files, imagery and tiles, Notebook workspaces) and your monthly transactions (geocoding, routes, drive-time areas, closest facility, multi-vehicle routes, GeoEnrichment, spatial analysis, tile generation, demographic maps, infographics, custom prints, ModelBuilder, AI image analysis, AI text translation), plus the credits your annual subscription includes, and get:

- The credit cost of every line item, with the biggest cost driver named
- Total credits per month and the annual projection
- Whether your annual credits cover the year, and how many months they last if they do not
- The two fixes that bring the bill down fastest, tied to your actual cost drivers

Three presets fill the form with typical months: a small team, a field data collection operation, and a routing-heavy operation. Change any number and the estimate follows. A print button produces a clean copy of the estimate.

## How it works

Single self-contained `index.html`. No backend, no API key, no account. The calculation runs entirely in your browser, and nothing you enter leaves the page.

## Sources

Every rate is Esri's published rate from the Understand credits documentation (doc.esri.com/en/arcgis-online/latest/administer/credits.html), checked 25 November 2026:

- Hosted feature storage: 2.4 credits per 10 MB stored per month
- File storage: 1.2 credits per 1 GB stored per month
- Imagery and tile storage: 1.2 credits per 1 GB stored per month
- Notebook workspace storage: 12 credits per 1 GB stored per month, per user
- Geocoding: 40 credits per 1,000 geocodes
- Simple routes: 0.005 credits per route
- Optimised routes: 0.5 credits per route
- Drive-time areas: 0.5 credits per area
- Closest facility routes: 0.5 credits per route
- Multi-vehicle routes: 1 credit per vehicle route
- GeoEnrichment: 10 credits per 1,000 attributes
- Spatial analysis: 1 credit per 1,000 features
- Tile generation: 1 credit per 10,000 tiles
- Demographic maps: 10 credits per 1,000 map requests
- Infographics: 10 credits per 1,000 views
- Custom layout prints: 5 credits per print job
- ModelBuilder: 50 credits per hour
- AI image analysis: 1 credit per 5 images
- AI text translation: 1 credit per 1,000 characters

Esri can change the rates, and real usage lives on the organisation status dashboard, so this is a planning estimate, not a bill. If a rate here disagrees with the documentation, the documentation wins.

## How to run it

Open `index.html` in any modern browser, or visit the live demo at https://janakigattu.github.io/projects/arcgis-online-credit-estimator/

## What to do next

Still unsure what your credits should cost? Email Janaki at gjanaki360@gmail.com with your monthly total and your biggest cost driver. Or book a session at https://janakigattu.github.io/#book and bring the numbers from your status dashboard.

# Field Data Collection Planner

The crew finds out the map does not work offline at the first dead zone, not in the office.

A working single-file web app that plans a Field Maps and Survey123 deployment before anyone leaves: the offline areas, the sync plan, the QA, and the setup effort, from the numbers you already know. No backend, no API key, no account. Everything runs in the browser, and nothing you enter leaves your device.

## What it does

Enter the crew size, devices, field days, records and photos per day, the number of forms, maps and offline areas, the basemap size, the connectivity in the field, the state of the feature service, the versioning model, and four ready checks. The planner returns:

- A readiness score out of 100, split across data readiness (30), offline setup (25), sync plan (20), QA and review (15), and devices and crew (10), with a verdict: Ready to go, Fix the gaps first, or Not ready, do the data work first.
- What the crew will collect: offline areas to build, records and photos expected, storage for records and photos, and the download size per device.
- A sync plan matched to the connectivity: auto-sync every 15 minutes where there is signal, manual sync at stops with signal where it is spotty, and an evening sync at base where there is none.
- The flags to close before the first field day, each with the fix: sync not enabled, mixed versioning, no offline areas, a basemap over 500 MB, fewer devices than crew, no reviewer, no pilot day, devices never tested with the real areas, no connectivity, a public survey, photo-heavy forms.
- A setup estimate in person-days across five workstreams, the biggest workstream named, the two fixes that cut the effort fastest, a five-phase plan, and a 12-item printable checklist.

Three presets: Small inspection crew, Utility asset survey, Disaster assessment. Clear all resets the form.

## Facts it rests on

- Field Maps auto-sync runs every 15 minutes while the app is open and connected, and it is on by default (Esri Field Maps documentation, Sync).
- Offline map areas are created in Field Maps Designer ahead of time, or on demand in the mobile app (Esri, Work offline with Field Maps).
- A mobile map package is read-only and does not support data collection, so map areas are the way to take editable data offline.
- Sync-enabled feature services need a Global ID field, archiving on non-versioned data (or a version for each downloaded map on versioned data), and one versioning model across the whole map. Hosted feature layers are already prepared; enable sync in the layer settings (Esri Support, Create Offline Areas in Referenced Feature Services).
- Survey123 collects data online or offline and syncs when connectivity is restored (Esri, ArcGIS Survey123 overview).

Day rates, storage figures (2 KB per record, 3 MB per photo), and score weights are planning rules from practice, stated as such on the page, not Esri numbers.

## How to run it

Open `index.html` in any browser. No build step, no server, no network calls. The Print plan button prints the plan.

## Sources

- https://doc.esri.com/en/arcgis-field-maps/latest/use-maps/sync.html?pivots=mobile-android
- https://www.esri.com/arcgis-blog/products/field-maps/field-mobility/work-offline-with-field-maps
- https://support.esri.com/en-us/knowledge-base/create-offline-areas-in-referenced-feature-services-usi-000039810
- https://www.esri.com/en-us/arcgis/products/arcgis-survey123/overview

## Call to action

Email Janaki with your crew size, your offline areas, and your readiness score, and she will tell you whether the deployment is a week of setup or a data project first: gjanaki360@gmail.com. Or book a session at https://janakigattu.github.io/#book.

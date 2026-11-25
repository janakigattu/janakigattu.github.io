# Esri COTS App Showcase

## Most teams do not need a custom app. They need the right Esri app, configured well.

Three patterns cover most of what a GIS team is asked to build. This page shows all three working, on the same live data, so a team can see the pattern before they commit to the product.

## What it does

Three working demos on one page, all reading Esri Living Atlas USA wildfire incidents live from ArcGIS Online:

1. **Experience Builder pattern.** A map, a list, a search box, and filters for state and size. Click a fire in the list and the map flies to it. This is the shape of most Experience Builder apps: a map widget, a list widget, and a filter widget, all reading the same layer.
2. **Dashboards pattern.** Four indicators (incidents, total acres, largest fire, average containment), a bar chart of acres by state, and a table of the ten largest fires. Every number is computed from the data when the page loads, and a refresh button re-queries the service.
3. **StoryMaps pattern.** Six chapters, generated from the five largest fires in the live data. Step through them and the map moves with the story, opening the pop-up for each fire.

A section at the bottom gives the build steps for each pattern in ArcGIS Online or ArcGIS Enterprise: which template, which widgets, and what to watch for. No custom code in any of them. That is the point.

## Data

Esri Living Atlas, USA Wildfires (Current Incidents): `services1.arcgis.com/P946On66WOQ606jN/arcgis/rest/services/USA_Wildfires_JF/FeatureServer/0`. One query returns at most 1,000 features, so the page loads the 1,000 largest incidents by acres and says so on the page. If the service does not answer, the panels say so instead of showing stale numbers.

## How to run it

Open `index.html` in a browser, or serve the folder with any static server. No build step, no backend, no API key. The map tiles come from Esri World Topo Map, the data comes from the Living Atlas service, and the mapping library is Leaflet with a small amount of plain JavaScript.

## Why this matters

Teams waste months building custom apps for jobs Esri already solved. Experience Builder covers find-it-and-open-it. Dashboards covers how-are-we-doing. StoryMaps covers follow-the-story. Knowing which pattern fits which question is the skill, and it is what fifteen years of enterprise GIS teaches. This page is the proof, working in the browser.

## Next step

If your team needs one of these three apps built on your data, email Janaki at gjanaki360@gmail.com or connect with her on LinkedIn at https://www.linkedin.com/in/janaki-gis-enterprise.

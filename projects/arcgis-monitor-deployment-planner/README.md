# ArcGIS Monitor Deployment Planner

Most Enterprise GIS teams only discover they have no monitoring when the map stops and nobody can say why. This planner fixes that before it happens.

## What it does

Enter the shape of your ArcGIS Enterprise deployment: Portal machines, Server machines, Data Store machines, extra server roles, enterprise geodatabases, networks, web adaptors, services, and users. Tick what Monitor should watch, how alerts should reach people, and five readiness checks. You get a deployment plan: Monitor Server only, or Monitor Server plus one Monitor Agent per extra network; the components to register, counted by group; a starter alert set with thresholds; four collections to build; the gaps to close before you deploy; a phased plan with a person-day estimate; and a printable checklist.

## How it works

A single self-contained `index.html`. No backend, no API key, nothing leaves the browser. Three presets (Small single site, Department multi-site, Enterprise distributed) fill the form, or enter your own numbers. The deployment shape, the component list, and the roles come from Esri's published ArcGIS Monitor documentation. The starter alert thresholds and the effort figures are planning rules from practice, labelled as such on the page: run the two-week baseline first, then tune the thresholds to your own numbers.

## Try it

Open `index.html` in any browser, or use the live page: https://janakigattu.github.io/projects/arcgis-monitor-deployment-planner/

## Companion reading

- ArcGIS Monitor guide (PDF): https://janakigattu.github.io/resources/arcgis-monitor-guide.pdf
- Enterprise GIS Health Check agent: https://janakigattu.github.io/projects/enterprise-gis-health-check-agent/
- Esri, Introduction to ArcGIS Monitor: https://doc.arcgis.com/en/monitor/2025.1/get-started/linux/

## Next step

Email Janaki with your machine count and your networks, and she will scope the deployment with you: gjanaki360@gmail.com. Or book a session from the portfolio home page.

# ArcGIS Migration Effort Estimator

Moving between ArcGIS Enterprise and ArcGIS Online is not one job. It is a pile of small jobs wearing one name, and the pile is different every time. This estimator counts what you actually have to move and prices the move in person-days, before anyone picks a tool.

## What it does

Enter the direction (ArcGIS Enterprise to ArcGIS Online, or ArcGIS Online to ArcGIS Enterprise), count your content (hosted feature services, web maps, Experience Builder apps, dashboards, StoryMaps, Web AppBuilder apps, scene layers, notebooks, named users, groups), and tick what else is in the estate (Utility Network, branch-versioned data, Server extensions or SOEs, GeoEvent feeds, no Python capacity, content never audited). You get:

- A person-day estimate, low to high, with the work broken out across eight workstreams
- A verdict: Straightforward, Tight but doable, or Rebuild-first
- Calendar weeks for one person and for a team of three
- The biggest workstream named, and the two fixes that cut the effort fastest
- The flags that set the schedule, with what each one changes
- A recommended approach for the direction you picked
- A phased plan sized to the numbers you entered, and a printable checklist

Three presets (Small department, Mid-size organisation, Large enterprise) fill the form. Clear all starts over.

## What it is built on

The scope-first thinking comes from Janaki's article [ArcGIS Enterprise Migration: Start With Scope, Not the Tool](https://www.linkedin.com/pulse/arcgis-enterprise-migration-start-scope-tool-janaki-gattu-g8xnc/) (LinkedIn, 24 November 2026): migration is four kinds of work, the platform-change kind is the one this estimator prices, and rebuilding a retired app type is its own workstream. WebGISDR rules come from Esri's [Migrate ArcGIS Enterprise with WebGISDR](https://doc.esri.com/en/arcgis-enterprise/latest/deploy/migrate-to-new-machines-with-webgisdr.html) documentation, and distributed collaboration from Esri's [Get started with distributed collaboration](https://learn.arcgis.com/en/projects/get-started-with-distributed-collaboration/) tutorial.

The day rates are planning rules from practice, not Esri numbers: Esri publishes no migration effort rates. The page says so plainly. If a rate disagrees with your own history, your history wins.

## How to run it

Open `index.html` in a browser. It runs entirely in the browser: no server, no API key, no account, and nothing you enter leaves the page. Print from the page for a paper copy of the estimate.

## What to do next

Email Janaki with your direction, your total, and your biggest workstream, at [gjanaki360@gmail.com](mailto:gjanaki360@gmail.com), or [book a session](https://janakigattu.github.io/#book) and bring the inventory from your portal.

# Utility Network Migration Planner

A trace returns the wrong customers, and nobody notices until someone who knows the field checks it. This planner prices the migration before a single feature moves, so the model gets decided first and the data move follows it.

## What it does

Enter your utility domain (electric, water, gas, wastewater, telecom), your source data (geometric network, file geodatabase, shapefiles and CAD, or mixed), and count what you have: source classes to map, total network features, subnetworks, editors, and the services and apps that consume the network. Pick a migration approach (Migration Wizard, Migration toolset, or Utility Network Foundations), state the connectivity failure rate in the source data, tick the Four-Gate Load Check from Janaki's Utility Network article, and say whether ArcGIS Enterprise, branch versioning, and operator involvement are already in place. You get:

- A person-day estimate, low to high, with the work broken out across nine workstreams
- A verdict: Ready to migrate, Migrate one part first, or Model first
- Calendar weeks for one person and for a team of three
- The biggest workstream named, and the two fixes that cut the effort fastest
- The flags that set the schedule, with what each one changes
- A seven-phase plan sized to the numbers you entered, and a printable checklist

Three presets (Small water district, Mid-size electric utility, Large enterprise) fill the form. Clear all starts over.

## What it is built on

The Four-Gate Load Check and the model-first order come from Janaki's article [ArcGIS Utility Network: Modernise the Model Before You Migrate the Data](https://www.linkedin.com/pulse/arcgis-utility-network-modernise-model-before-you-migrate-gattu-z6vuc/) (LinkedIn, 24 November 2026): settle what the network is for, test what the data actually says, and agree how editors will work in it, before choosing the loading method or the cutover date. The three migration approaches, the Analyze Network Data and Apply Error Resolutions tools, and the branch versioning requirement come from Esri's [Migrate existing data into a utility network](https://pro.arcgis.com/en/pro-app/3.5/help/data/utility-network/migrate-existing-data.htm) and [Utility network FAQ](https://pro.arcgis.com/en/pro-app/3.3/help/data/utility-network/faq.htm) documentation. The four-trace test comes from the [Utility Network Tracing Demo](https://janakigattu.github.io/projects/utility-network-tracing-demo/) on this portfolio.

The day rates are planning rules from practice, not Esri numbers: Esri publishes no migration effort rates. The page says so plainly. If a rate disagrees with your own history, your history wins.

## How to run it

Open `index.html` in a browser. It runs entirely in the browser: no server, no API key, no account, and nothing you enter leaves the page. Print from the page for a paper copy of the plan.

## What to do next

Email Janaki with your total person-days and your biggest workstream, at [gjanaki360@gmail.com](mailto:gjanaki360@gmail.com), or [book a session](https://janakigattu.github.io/#book) and bring the four gates, answered in writing.

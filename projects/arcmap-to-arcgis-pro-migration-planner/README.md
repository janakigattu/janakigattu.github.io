# ArcMap to ArcGIS Pro Migration Planner

ArcMap retired on March 1, 2026, and the maps, scripts, and custom tools built on it did not retire with it. This planner counts an ArcMap estate, prices the move to ArcGIS Pro in person-days, names the compatibility flags that set the schedule, and prints a phased plan with a checklist.

## What it does

Enter your ArcMap estate: map documents (.mxd, .sxd, .3dd), map complexity, Python 2 scripts, ModelBuilder models, custom .NET add-ins and ArcObjects tools, map services published from ArcMap, Pro users to train, ArcMap version, and licence type, plus five known blockers (personal geodatabases, geometric networks, ArcMap-based extensions, VB expressions in Calculate Field, ArcScene and ArcGlobe documents). Three presets cover a small team, a mid-size department, and a large enterprise.

The planner returns:

- A person-day estimate, low to high, broken down by nine workstreams: inventory, map conversion, Python migration, model rebuild, custom tool rebuild, service republication, training, validation, and cutover.
- A calendar estimate for one person and for a team of three.
- A verdict: Straightforward, Tight but doable, or Rebuild-first.
- Compatibility flags with the fix for each one, including the subscription-licence warning that access to ArcMap ends when the subscription expires.
- The two fixes that cut the effort fastest, chosen from the biggest workstreams.
- A seven-phase plan (inventory, pilot, convert, rebuild, validate, train and cut over, retire ArcMap) sized to the numbers entered, and a 14-item printable checklist.

## Sources

Compatibility rules come from Esri's published migration guidance, checked 25 November 2026:

- ArcGIS Desktop retirement, Esri Support: ArcMap retired March 1, 2026; 10.8.2 was the final release; no patches or hot fixes after retirement.
- ArcGIS Desktop retirement, plan your migration, Esri: migrating customers move to Creator, Professional, and Professional Plus user types.
- Migrate existing work, ArcGIS Pro documentation: Import Map tool, styles (.style to .stylx), Python 2.7 to Python 3 with arcpy.mapping replaced by arcpy.mp, .NET add-ins written for ArcMap will not run in Pro, geometric networks convert to trace networks.
- Automate conversion of ArcMap MXDs to ArcGIS Pro projects, Esri Support: batch MXD to APRX conversion with arcpy.mp and importDocument.

Effort ranges are planning estimates from typical migration work, not Esri figures. The page says so plainly. Treat them as the size of the job, not the price of it.

## How to run it

Open `index.html` in any browser. No server, no API key, no account, and nothing entered leaves the page. Click "Build my migration plan", or pick a preset. "Print my plan" prints the plan and checklist.

## Built by

Janaki Gattu, Enterprise GIS Consultant and GIS Solutions Architect. Questions about your migration, or want someone who has done this to run it? Email gjanaki360@gmail.com or connect on LinkedIn at https://www.linkedin.com/in/janaki-gis-enterprise.

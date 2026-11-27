# Enterprise Geodatabase Design Planner

The versioning choice you make on day one decides what your editors can and cannot do for the next ten years. Get it right before the first dataset is registered.

## What it does

Answer ten questions about how your team edits, and get the enterprise geodatabase design: branch or traditional versioning (or a split of both), archiving, editor tracking, replicas, offline editing, and the maintenance the design needs. Conflicts are named before you build, not found after: a Utility Network with ArcMap editors still in use, or move edits to base with replication in scope, both stop the design and say what has to change.

Three presets cover the common shapes: a small team with one editor at a time, a department editing through web feature layers with replication, and an enterprise utility running a Utility Network across three sites. Every preset produces a different design, and the enterprise one is deliberately blocked by a real conflict.

## What you get

- A versioning recommendation with the rule behind it, for each decision
- A design readiness score out of 100 and a verdict: Ready to build, Decide the open points first, or Resolve the conflicts first
- A decision-by-decision table: versioning, archiving, editor tracking, copies and sync, offline editing, maintenance, version rules
- The gaps to close, each with the fix
- A build checklist in order, printable
- An effort estimate in person-days, labelled as a planning rule from practice

## How it works

Single self-contained page. No backend, no API key, nothing leaves your browser. The logic is a pure function, `computeDesign(d)`, so the design is reproducible from the same answers.

The rules come from Esri's published ArcGIS Pro documentation: branch versioning is the mechanism behind versioned web editing and the only option for Utility Network, parcel fabric, trace network, and topology; it needs global IDs and editor tracking in UTC, needs a geodatabase at release 10.6 or later, and ArcMap cannot open it (ArcGIS Pro 2.1 is the minimum). Geodatabase replication is built on traditional versioning and does not support branch versioned data in any replica type, nor move edits to base. Archiving is automatic with branch versioning and enabled separately on traditional and non-versioned data. A dataset can only be in one versioning type, so a mixed estate splits by dataset.

## Run it

Open `index.html` in any browser, or visit the live page on the portfolio site. Pick a preset or fill in your own numbers, then press "Design my geodatabase".

## Sources

- Versioning types: https://pro.arcgis.com/en/pro-app/latest/help/data/geodatabases/overview/versioning-types.htm
- Register a dataset as branch versioned: https://doc.esri.com/en/arcgis-pro/latest/help/data/geodatabases/overview/register-a-dataset-as-branch-versioned.html
- Enable archiving: https://doc.esri.com/en/arcgis-pro/latest/help/data/geodatabases/overview/enabling-archiving.html
- Enable editor tracking: https://doc.esri.com/en/arcgis-pro/latest/help/data/geodatabases/overview/enable-editor-tracking.html
- Replication and geodatabase compatibility: https://pro.arcgis.com/en/pro-app/3.2/help/data/geodatabases/overview/replication-and-geodatabase-compatibility.htm

## Call to action

Ready to build it? Email Janaki with your dataset count and editor count and she will walk the design through with you: gjanaki360@gmail.com, or book a session at https://janakigattu.github.io/#book.

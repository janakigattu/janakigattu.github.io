# GIS Data Quality Scorecard

Every migration, upgrade, and AI pilot your team plans is priced on the data you have. Ten questions show whether that data is worth the price.

## What it does

A guided assessment that scores one dataset, or one estate of datasets, on data quality. Answer 10 questions across 6 areas and get a score out of 100, a red, amber, or green status per area, the top 3 gaps to close with a fix for each, recommended next steps, and your full answer list. Restart any time.

The six areas:

1. **Completeness** (2 questions): required attributes populated, and records with missing or broken geometry counted.
2. **Accuracy** (2 questions): positional accuracy verified against a control source, and attribute values checked against the source system.
3. **Currency** (2 questions): an update schedule that is met, and last-updated dates so stale records can be spotted.
4. **Consistency** (1 question): naming, domains, and coordinate systems consistent across datasets.
5. **Lineage and documentation** (2 questions): source and processing steps recorded, and metadata that matches the data as it is today.
6. **Fitness for use and QA** (1 question): automated checks on a schedule, and known limitations written down where users can see them.

## How to run it

Open `index.html` in any browser. No server, no build step, no API key, and nothing you answer leaves the page. The score is calculated in the browser and is not stored or sent anywhere.

## What it is built from

Janaki Gattu's migration article (LinkedIn, 24 Nov 2026), which starts with scope before the tool, and Esri's ArcGIS Data Reviewer documentation on automated checks, error management, and data quality reporting: https://doc.esri.com/en/arcgis-data-reviewer/latest/get-started/what-is-arcgis-data-reviewer-for-server.html

The two checks the scorecard tells you to automate first, blank required fields and null geometry, are the same checks the Notebook Automation Gallery on this portfolio runs on sample data.

## What it is not

This check is a starting point. It scores what you tell it about your data; it does not read your data. A full data quality review tests the data itself, in your own environment, with the checks configured for your rules.

## Next step

Email Janaki at gjanaki360@gmail.com with your score and your top gap, or book a session on her portfolio at https://janakigattu.github.io/#book

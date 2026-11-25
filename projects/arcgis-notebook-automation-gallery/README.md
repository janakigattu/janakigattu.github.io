# ArcGIS Notebook Automation Gallery

Nobody schedules a meeting to check for duplicate IDs. That is exactly why a notebook should do it at 2 a.m.

## What it is

Four working ArcGIS Notebook automations on one page, each running for real in the browser on a small sample dataset:

1. **Nightly Data QA Check** (daily, 02:00): 12 asset records checked for missing geometry, blank required fields, duplicate IDs, and edits older than 180 days. Result: 9 issues, 4 of 12 records clean.
2. **Weekly User and Content Audit** (Mondays, 07:00): 10 users and 8 items checked for dormant members (no sign-in for 90 days), items never shared, and items with no views in 180 days. Result: 10 findings.
3. **Scheduled Layer Sync** (every 6 hours): 14 source rows compared against 12 target rows by business key. Result: 2 inserts, 2 updates, 1 delete, 10 unchanged, target ends at 14 rows.
4. **Monthly Service Health Report** (1st of the month, 06:00): 8 services measured on uptime, response time, and errors. Result: 99.80 percent average uptime, 2 services below the 99.5 percent target, slowest is Permits at 1,450 ms, 139 errors in 30 days.

Each notebook has a **Run it now** button that prints a timestamped run log step by step and renders a results panel, plus a **copyable Python skeleton** using the ArcGIS API for Python (`GIS("home")`, content search, feature layer query and `edit_features`, users search). A weekly schedule strip shows which notebooks run on which days, and a four-step section explains how a scheduled notebook works on ArcGIS Notebook Server.

## How it runs

Single self-contained `index.html`. No backend, no API key, no account, nothing leaves the page. Open it in any browser and click Run it now on any notebook.

## Sources

- Esri: Schedule a notebook task, ArcGIS Notebook Server 12.0 — https://enterprise.arcgis.com/en/notebook/12.0/use/windows/prepare-a-notebook-for-automated-execution.htm (scheduling available from Enterprise 10.8.1; Tasks pane; parameters inserted as a cell; no user interaction while a scheduled run executes)
- ArcGIS API for Python — https://developers.arcgis.com/python/
- Sample datasets on the page are small, made-up records built to show each check working. The Python skeletons take your own layer item ids, field names, and thresholds.

## What to do next

Pick the notebook your team needs first. Most teams start with the nightly QA check, because bad data is the problem that quietly corrupts everything downstream. Email Janaki at gjanaki360@gmail.com with the manual job your team repeats every week, or book a session at https://janakigattu.github.io/#book and she will scope the notebook that replaces it.

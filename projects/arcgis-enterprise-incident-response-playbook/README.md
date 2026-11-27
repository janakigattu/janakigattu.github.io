# ArcGIS Enterprise Incident Response Playbook

An outage is not the time to work out what to do next. This is the page you open when the system is down.

## What it does

Pick the incident (Portal will not load, services slow or timing out, sign-in failing, data store read-only or disk full, federation broken, restore from backup with WebGISDR), answer five questions about the situation, and get a playbook: the severity (SEV-1, SEV-2, or SEV-3) with the response target and who to page, the runbook steps in order with the check that confirms each one, the warnings that apply to this incident, a status message ready to copy and send to users, and a post-incident review checklist. Print button included. Three presets cover the common cases.

## How it runs

Single self-contained HTML file. No backend, no API key, nothing typed is sent or stored anywhere. Open `index.html` in a browser.

## What it is built on

Severity bands and response targets are planning rules from practice, not Esri numbers, and the page says so. The runbook steps come from Esri published guidance:

- Esri, ArcGIS Enterprise backups and WebGISDR restore (settings that must match between environments, what the restore keeps from the target): enterprise.arcgis.com/en/portal/11.5/administer/linux/overview-backup-restore-web-gis.htm
- Esri, ArcGIS Data Store system requirements (below 10 GB free the data store logs warnings, below 5 GB free the relational store goes read-only): enterprise.arcgis.com/en/data-store/latest/install/windows/arcgis-data-store-system-requirements.htm
- Esri, ArcGIS Monitor (alerts fire when a metric crosses a threshold): doc.arcgis.com/en/monitor/latest/get-started/introduction-to-arcgis-monitor.htm

Related tools on the portfolio: the ArcGIS Enterprise Troubleshooting Agent (find the cause), the WebGISDR Backup and Recovery Planner (the backup schedule this playbook assumes), and the ArcGIS Monitor Deployment Planner (the alerts that should have fired).

## What to do next

Run it against your own deployment and check the severity it gives for the incident you fear most. Then email Janaki with the incident, the severity, and the step where the runbook stopped working: gjanaki360@gmail.com, or book a session at janakigattu.github.io.

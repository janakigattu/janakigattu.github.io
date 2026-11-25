# WebGISDR Backup and Recovery Planner

Your last good backup is the only version of your organisation you can get back. This planner shows whether that backup actually exists, what it does not cover, and how to restore it when the day comes.

## What it does

Answer five short sections about your ArcGIS Enterprise deployment and get a backup plan in about three minutes:

- **A readiness score out of 100**, with the breakdown: deployment pattern (20), backup storage (15), five readiness answers (40), and coverage of what you run (25). 80 and above is Recoverable, 50 to 79 is Partly covered, below 50 is At risk.
- **A recommended schedule**: full backup cadence plus incremental cadence, set by how fast your content changes. Heavy change gets the pattern Esri documents, a full backup at midnight and incrementals at 10:00 a.m., 2:00 p.m., and 6:00 p.m. Replicated deployments get the four-scripts-plus-cron pattern with the 30 to 60 minute buffer.
- **What WebGISDR covers, and what it does not**: portal items and settings, GIS services and settings, service webhooks, and the relational, tile cache, object, and graph data stores are in the backup. Cache tiles, referenced data, enterprise geodatabases, the spatiotemporal big data store, GeoEvent and Mission Server configuration, and the Notebook Server workspace directory are not, and the planner lists the separate backup each one needs.
- **A webgisdr.properties starter**, generated from your answers: backup mode, store provider, and shared location filled in, with the incremental variant noted.
- **A printable restore checklist**, from confirming the target version and URLs to the post-restore smoke test and recording the real recovery time.

## How it runs

A single self-contained `index.html`. No backend, no API key, no account. Everything is calculated in the browser and nothing you answer leaves the page. Open the file in any browser, or use the live demo below.

## Grounded in

Esri's published WebGISDR documentation: the ArcGIS Enterprise backups overview (what is included, what is not, backup modes, and the settings that must match between environments) and the automated replication guide (full and incremental properties files, four scripts, cron scheduling, and the 30 to 60 minute buffer). Links to both are on the page.

## Live demo

https://janakigattu.github.io/projects/webgisdr-backup-recovery-planner/

## Call to action

A plan on paper is worth less than one restore test. Email Janaki Gattu at gjanaki360@gmail.com with your score and she will help you set the schedule up, test the restore, and close the gaps. Or book a session from the portfolio home page.

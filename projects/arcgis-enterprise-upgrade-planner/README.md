# ArcGIS Enterprise Upgrade Planner

Most failed upgrades are not installer errors. They are version jumps Esri never supported, taken without a backup.

## What it does

A working upgrade planner that runs entirely in your browser. Enter your current version and your target version, plus your deployment pattern, the extra server roles you run, and five honest readiness questions. It gives you:

- **The upgrade path Esri supports.** A direct upgrade where one is supported, or the interim versions where it is not. Built from Esri's published direct-upgrade table: 11.0 to 11.5 go direct to 12.0, 10.8 to 10.9.1 go direct to 11.5, 10.7 to 10.7.1 go direct to 11.3.
- **The traps that change the path.** Hosted scene layers and Web AppBuilder apps force an 11.5 stop before 12.0, with the cache migration and the Experience Builder rebuild spelled out. Features retired at 11.0 are flagged when you are jumping from 10.9.1 or earlier.
- **A readiness score out of 100.** Staging rehearsal, a proved webgisdr backup, system requirements checked, custom apps inventoried, and a maintenance window agreed. The two that matter most, staging and backup, are called out when they are missing.
- **A checklist you can run.** Phase 0 preparation, one phase per version step in Esri's component order (Portal, Web Adaptor for Portal, hosting Server, Web Adaptor for Server, Data Store, then each extra server role and federated site), validation, and the rollback. Tick each step off as you go, and print the plan.
- **A planning estimate for the window.** Based on your deployment pattern and the number of version steps, plus a validation window on top. Labelled as an estimate, not a promise.

## How to run it

Open `index.html` in any browser. No server, no backend, no API key, nothing you enter leaves the page.

## Sources

Esri, "Upgrade ArcGIS Enterprise" and "Prepare to upgrade ArcGIS Data Store", enterprise.arcgis.com. The direct-upgrade table, the component order, the 12.0 interim-version rule, the hosted scene layer cache rule, and the same-version rule are all from Esri's published upgrade documentation. Check the documentation for your exact target version before you start.

## Who built it

Janaki Gattu, Enterprise GIS Consultant and GIS Solutions Architect, with 15+ years in enterprise GIS and 10 years administering ArcGIS Enterprise, including upgrades at Caltrans.

## Next step

If your team would rather have someone who has done this before run the upgrade, that is what Janaki does. Email gjanaki360@gmail.com or connect on LinkedIn at https://www.linkedin.com/in/janaki-gis-enterprise.

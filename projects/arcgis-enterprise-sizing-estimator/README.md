# ArcGIS Enterprise Sizing Estimator

Most Enterprise GIS servers are sized by habit: whatever the last project bought. Size yours from the load instead.

## What it does

Enter your named users, peak concurrent users, concurrent editors, hosted feature services, data volumes (relational data, tile cache, file uploads), extra server roles, and availability need, and get the deployment pattern (single machine, base, or highly available), the spec for every machine (cores, RAM, disk), the totals, the flags that change the answer, and a printable spec sheet. Three presets cover a small team, a department, and an enterprise.

## How it works

The sizing starts from Esri's published 11.5 minimums and scales up from the load with planning rules that are labelled as rules, not Esri numbers:

- Portal for ArcGIS 11.5: 2 cores minimum, 4 highly recommended for production, 8 GB RAM, 20 GB disk. The estimator scales Portal with named users: 4 cores and 8 GB RAM up to 250 users, 8 cores and 16 GB up to 1,000, 16 cores and 32 GB above that. Disk is 20 GB plus your file volume.
- ArcGIS Server 11.5 (hosting): 8 GB RAM per machine minimum, 10 GB disk, and Esri publishes no production numbers. The estimator scales the hosting server with peak concurrent users and editors: 4 cores and 8 GB up to 50 concurrent, 8 cores and 16 GB up to 200, 16 cores and 32 GB above, plus 4 cores and 8 GB when more than 25 people edit at once. Disk is 10 GB plus 10 GB per 100 services.
- ArcGIS Data Store 11.5: 13 GB disk to install one empty type, minimum free RAM of 8 GB for a relational store and 8 GB for a tile cache store. The estimator scales the relational store with data volume: 8 GB RAM up to 25 GB, 16 GB up to 100 GB, 32 GB up to 500 GB, 64 GB above. Disk is install 13 GB plus one copy live, one copy growth headroom, and one copy backup.
- A single machine carries everything, so its RAM and disk add up and its cores take the hosting server number plus four for Portal and the data store. A highly available deployment doubles every core machine and adds a load balancer and shared storage.
- Each extra federated role (GeoEvent, Notebook, Image, Workflow Manager, GeoAnalytics) gets its own machine at the ArcGIS Server minimum or above.

Flags call out the decisions that matter: a single machine at real load, tile caches on slow disk, editor peaks, the 10 GB free disk warning line below which Esri logs warnings, and the 5 GB line below which the stores go read-only.

## Sources

- Portal for ArcGIS 11.5 system requirements: https://enterprise.arcgis.com/en/system-requirements/11.5/windows/portal-for-arcgis-system-requirements.htm
- ArcGIS Server 11.5 system requirements: https://enterprise.arcgis.com/en/system-requirements/11.5/windows/arcgis-server-system-requirements.htm
- ArcGIS Data Store 11.5 system requirements: https://enterprise.arcgis.com/en/system-requirements/11.5/windows/arcgis-data-store-system-requirements.htm

## How to run it

Open `index.html` in a browser. No backend, no API key, nothing is sent anywhere. Use the Print button for a spec sheet to take to procurement.

## What to do next

Email Janaki your totals (machines, cores, RAM, disk) and she will sense-check the spec before you buy hardware: gjanaki360@gmail.com. Or book a session at https://janakigattu.github.io/ and walk through the load together.

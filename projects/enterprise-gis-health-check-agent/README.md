# Enterprise GIS Health Check Agent

A working, single-file web assessment by Janaki Gattu. It helps an ArcGIS Enterprise team find the cracks in their platform before they break, and it produces a readiness report they can act on.

## What the agent does

The visitor answers 10 short questions, one at a time, across 7 platform health areas:

1. Uptime and monitoring
2. Backups and disaster recovery
3. Security and access control
4. Data quality
5. Performance
6. Upgrades and patches
7. Documentation and governance

At the end it shows:

- A total score out of 100 (each question is worth up to 10 points)
- A red, amber, or green status for each of the 7 areas (green 75% or higher, amber 50 to 74%, red below 50%)
- The top 3 gaps to close, taken from the lowest-scoring answers, each with a concrete fix
- Recommended next steps: start with one area this week, turn the gaps into a short ranked fix list with an owner and a date for each item, and repeat the check on a quarterly rhythm, with a deeper check once a year
- A full list of the visitor's answers, and a restart button

## Hook and call to action

Hook, at the top of the page: "Most teams only check their ArcGIS Enterprise deployment after something breaks, usually on a Monday morning. Take ten minutes now and find the cracks before they break."

Call to action, on the results screen: email Janaki at gjanaki360@gmail.com with the score, or book a session at https://janakigattu.github.io/#book. The page also links back to the portfolio at https://janakigattu.github.io/.

## How to use it

Open `index.html` in a browser. No build step, no install, no account. Click "Start the health check", answer each question, and read the report. Click "Restart the health check" to run it again.

The page states honestly that it runs entirely in the browser with no backend and no API key, and that nothing answered leaves the page. Scores are calculated in the browser and are not stored or sent anywhere.

## Content source

Questions and guidance come from the Enterprise GIS Weekly episode "ArcGIS Enterprise Health Check: Find the Cracks Before They Break" and Janaki Gattu's work administering ArcGIS Enterprise: monitoring and alerts, logs nobody reads, services that need routine restarts, broken layers and unowned content, permissions creep, backups never restored, restore time nobody can state, slow services, patch lag, and runbooks and governance. No product claims, certifications, or statistics were invented.

## Files

- `index.html` — the complete app: HTML, CSS, and JavaScript in one self-contained file
- `README.md` — this file

## Live path

`projects/enterprise-gis-health-check-agent/index.html`

## Visual style

Matches the existing Enterprise GIS AI Assistant demo: dark background (#0a0a0a), cards (#161616), green accent (#4ade80), amber (#fbbf24), system font stack.

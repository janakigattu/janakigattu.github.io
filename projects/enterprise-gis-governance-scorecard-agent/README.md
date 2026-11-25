# Enterprise GIS Governance Scorecard Agent

A working, single-file web assessment by Janaki Gattu. It helps an ArcGIS Enterprise team see whether their platform is governed or just running on habit, and it produces a readiness report they can act on.

## What the agent does

The visitor answers 10 short questions, one at a time, across 7 governance areas:

1. Roles and ownership
2. Access and sharing
3. Standards and naming
4. Data lifecycle
5. Content management
6. Change control
7. Audit and compliance

At the end it shows:

- A total score out of 100 (each question is worth up to 10 points)
- A red, amber, or green status for each of the 7 areas (green 75% or higher, amber 50 to 74%, red below 50%)
- The top 3 gaps to close, taken from the lowest-scoring answers, each with a concrete fix
- Recommended next steps: start with one area this week, turn the gaps into a short ranked fix list with an owner and a date for each item, and repeat the check on a quarterly rhythm, with a deeper check once a year
- A full list of the visitor's answers, and a restart button

## Hook and call to action

Hook, at the top of the page: "Governance is invisible when it works, and expensive when it does not. Ten questions show which one you have."

Call to action, on the results screen: email Janaki at gjanaki360@gmail.com with the score, or book a session at https://janakigattu.github.io/#book. The page also links back to the portfolio at https://janakigattu.github.io/.

## How to use it

Open `index.html` in a browser. No build step, no install, no account. Click "Start the governance scorecard", answer each question, and read the report. Click "Restart the governance scorecard" to run it again.

The page states honestly that it runs entirely in the browser with no backend and no API key, and that nothing answered leaves the page. Scores are calculated in the browser and are not stored or sent anywhere.

## Content source

Questions and guidance come from Janaki Gattu's work administering ArcGIS Enterprise and her migration article, which starts with scope, owners, and the questions to answer in writing before you choose a tool, plus Esri's administration guidance on member roles and groups (Configure member roles and Manage groups, doc.arcgis.com). No product claims, certifications, or statistics were invented.

## Files

- `index.html`: the complete app: HTML, CSS, and JavaScript in one self-contained file
- `README.md`: this file

## Live path

`projects/enterprise-gis-governance-scorecard-agent/index.html`

## Visual style

Matches the existing Enterprise GIS Health Check agent: dark background (#0a0a0a), cards (#161616), green accent (#4ade80), amber (#fbbf24), system font stack.

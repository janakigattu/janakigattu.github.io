# ArcGIS Enterprise Troubleshooting Agent

The map stopped loading at 4:55 pm on a Friday. This agent finds the cause before the phone starts ringing.

## What it does

A working diagnostic agent for ArcGIS Enterprise. Pick one of six symptoms, answer three questions, and get the most likely cause, the checks that confirm it, and the fix, with the Esri documentation behind every answer.

The six symptoms:

1. Portal or ArcGIS Server will not start, or a service will not start
2. Maps and apps load slowly or time out
3. Users cannot sign in, or get access denied
4. Federating a server fails, or the hosting server shows errors
5. Publishing a service fails
6. A WebGISDR backup or restore fails, or never finishes

Each symptom has its own decision tree: three questions, weighted answers, and three or four ranked causes. The result names the most likely cause, the checks that confirm it, the fix in steps, a second cause worth checking, and when to open a case with Esri Support, including the four things Support asks for first.

## How it works

Single self-contained `index.html`. No backend, no API key, no account. The decision tree runs entirely in the browser, and nothing you answer leaves the page. If your answers do not point at one cause, the agent says so and gives the three first checks: disk space, the logs, and what changed.

## Sources

Every cause is grounded in Esri's own administration guidance, verified live on 2026-11-25:

- Esri: Common administration questions (ArcGIS Enterprise documentation): federation errors and the fully qualified domain name rule, SSL certificate recovery, sign-in and identity store behaviour, the relational Data Store going read-only below 1024 MB of free disk, publishing errors, and WebGISDR failures.
- Esri Support: the route for a failure the documentation does not cover.
- ArcGIS Monitor guide (Janaki Gattu, portfolio PDF): for the slow-map causes that need usage and performance numbers.

The agent also opens with the three questions that solve most failures: what changed, what do the logs say, and how much disk is free.

## How to run it

Open `index.html` in any modern browser, or visit the live demo at https://janakigattu.github.io/projects/arcgis-enterprise-troubleshooting-agent/

## What to do next

Still stuck after the fix? Email Janaki at gjanaki360@gmail.com with the symptom, the diagnosis the agent gave, and the exact error text from your log. Or book a session at https://janakigattu.github.io/#book and bring the failure with you: the version of every component, the error text, and what changed most recently.

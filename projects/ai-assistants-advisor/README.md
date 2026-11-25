# AI Assistants in GIS Advisor

A working single-file web app by Janaki Gattu. The visitor picks a task, and the advisor recommends the right ArcGIS AI assistant for it, with its availability, where it runs, and the admin opt-in caveat.

## What it does

Seven tasks are offered. Each one maps to a recommendation built only on the verified facts below:

| Task | Recommendation |
| --- | --- |
| Build a survey | Survey123 assistant — generally available, no extra cost |
| Translate content | Translation assistant — generally available, no extra cost |
| Analyse data for a report | Business Analyst assistant — generally available, no extra cost |
| Write Arcade expressions | Arcade assistant — beta / preview |
| Analyse data in a notebook | Notebooks assistant — beta / preview |
| Summarise a layer or item | Item details assistant — beta / preview; the only one in Enterprise, only in 12.0 |
| Draft a dashboard | No dedicated assistant is named for this in the verified list. The result says so plainly and suggests the closest honest option: the Business Analyst assistant, generally available at no extra cost, for the analysis behind the dashboard. |

Every result shows the availability (generally available vs beta / preview), whether it needs ArcGIS Online or Enterprise 12.0, and the admin opt-in caveat: access is governed at the organisation level, and an administrator must opt in to AI features.

## How to use it

1. Open `index.html` in any browser. There is no build step, no server, and no API key.
2. Pick a task from the list.
3. Read the recommendation, the availability badges, where it runs, the next step, and the admin opt-in caveat.
4. Click a task again to compare recommendations. Nothing you pick leaves the page.

## Files

- `index.html` — the whole app: HTML, CSS, and JavaScript in one self-contained file.
- `README.md` — this file.

## Live path

`projects/ai-assistants-advisor/index.html`

## Verified facts it is built on

From the portfolio's "Four topics, one carousel" slide, Topic 01 (AI Assistants in GIS), and Esri's "What's new in AI assistants" (June 2026):

- 12 AI assistants live inside ArcGIS.
- 3 are generally available at no extra cost: Survey123, Business Analyst, Translation.
- The rest are in beta or preview, including the Pro, Notebooks, and Arcade assistants.
- Most value today arrives through ArcGIS Online. The Item details assistant is the only one in Enterprise, and only in 12.0.
- Access is governed at the organisation level. An administrator must opt in to AI features.

No assistant name, feature, or availability status beyond these facts is used in the app. Where no named assistant exists for a task, the app says so instead of inventing one.

## Hook and call to action

- Hook (opening line): "Twelve assistants live inside ArcGIS. Pick the task, and this advisor tells you which one fits."
- Call to action (closing block): email Janaki at gjanaki360@gmail.com, and a Book a Session link to https://janakigattu.github.io/#book. The page also links back to the portfolio at https://janakigattu.github.io/.
- The app states honestly that it runs entirely in the browser with no backend and no API key.

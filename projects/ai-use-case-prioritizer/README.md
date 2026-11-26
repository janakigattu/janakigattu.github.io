# AI Use Case Prioritizer

Every team has ten ideas for AI and budget for one pilot. Pick the wrong first pilot and you burn the budget and the trust. Rank the candidates on value, data, effort, and risk, and start with the one that can actually ship.

## What it does

List up to six AI use cases, each with hours saved per person per week, people affected, data readiness, effort to build, and risk if it gets it wrong. The prioritizer scores each one out of 100, sorts them into four quadrants, and names the first pilot. It also gives the annual hours at stake for each candidate and what to do with each quadrant.

## How it works

- Three presets: a small team with four candidates, a support-heavy team with five, and a data-rich department with five. Every field is editable, and a row with no name is ignored.
- Scoring, stated on the page so you can disagree with it: weekly hours at stake is hours saved times people affected. Value, out of 50, is that number against the best candidate in the list. Feasibility, out of 50, is data readiness (0 to 20), effort inverted (0 to 15), and risk inverted (0 to 15). The priority score is value plus feasibility, out of 100.
- Quadrants: 25 or more on both halves is a Quick win, high value with low feasibility is a Strategic bet, low value with high feasibility is a Fill-in, low on both is Park it. Ties break on feasibility, then value.
- The recommended first pilot is the top-scoring Quick win. If there is no quick win, the top score leads, and the page says what to fix before piloting it.
- Output: a ranked table with value, feasibility, score, and quadrant per candidate, quadrant guidance, the success number in annual hours, and a print button.

## Running it

Open `index.html` in any browser. It runs entirely in your browser. There is no server, no API key, no account, and nothing you enter leaves the page.

## Sources

Built from the Harness Readiness Check in Janaki's article "Harness Engineering: The Discipline That Separates Production AI from Demos" (LinkedIn, 24 November 2026): build the harness with the first version around one small task, and judge the pilot on a verifiable outcome. The scoring weights are planning rules from practice, not Esri or vendor numbers. The next step after this ranking is the AI Pilot Planner, and the readiness check that comes before it is the AI Readiness Assessment.

## What to do next

Take the top-ranked use case to the AI Pilot Planner and turn it into a 30-day plan with a success number and a go or no-go call. Or email Janaki with your top pick and its score, and she will tell you what to fix first.

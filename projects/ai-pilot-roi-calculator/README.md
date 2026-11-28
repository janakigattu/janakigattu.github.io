# AI Pilot ROI Calculator

The pilot saved hours. The finance question is when it pays for the build. This calculator takes the pilot's measured hours saved, the rollout size and adoption, the running cost, and the one-off build and training cost, and gives back the payback in months, the annual net value, and the two levers that move the answer fastest.

## What it does

- Enter what the pilot proved (hours saved per user per week, pilot users), the rollout (total users, expected adoption, loaded hourly rate), the running cost (model and hosting per month, review hours per week, reviewer rate), and the one-off cost (build cost, training hours per user).
- Output: payback in months, verdict (Pays for itself fast / in year one / in year two / Does not pay yet), annual hours saved, gross value, annual running cost, net annual value, year-one net, ROI in year one, a line-by-line money table, the biggest year-one cost named, the payback at half adoption, and two levers (adoption to 100%, review hours halved) with the months each saves.
- Three presets: Small team document intake (1.2 months payback), Department support assistant (1.9 months), Regulated rollout, review-heavy (4.0 months). Clear all resets to zero.
- Print button for the summary.

## How it works

- Runs entirely in the browser. No server, no API key, no account, nothing entered leaves the page.
- Value is hours saved x users x adoption x 48 working weeks, priced at the loaded hourly rate. Running cost is model and hosting plus review hours. One-off cost is build plus training (users x hours x rate).
- Payback is the one-off cost divided by the monthly net value. The verdict bands are 6, 12, and 24 months.
- The 48 working weeks, the review rate, and the verdict bands are planning rules from practice, stated on the page. The hours saved, rates, and costs are yours.

## Sources

- Harness Engineering article (LinkedIn, 24 Nov 2026): judge the pilot on a verifiable outcome.
- AI Cost Estimator on this portfolio: price the monthly model and hosting line.
- AI Assistant Rollout Planner on this portfolio: wave sizing and review capacity.

## Live demo

https://janakigattu.github.io/projects/ai-pilot-roi-calculator/

## Next step

Email Janaki with the payback in months and the net value a year, and she will check the numbers against the pilot before the budget goes in: gjanaki360@gmail.com, or book a session at https://janakigattu.github.io/#book.

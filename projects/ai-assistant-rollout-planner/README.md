# AI Assistant Rollout Planner

The pilot worked for five people. Now fifty want the assistant, and the rollout is where pilots go to die. Plan the waves, the review capacity, and the training before you switch the whole team on.

## What it does

Enter what the pilot proved (hours saved per user per week, pilot users), the rollout size (total users, teams), the data and guardrails (sensitivity, data sources, the four harness gates, announcement and support channel), and the review and training picture (named reviewers, reviews per reviewer per day, expected requests per day, training hours per user, champions). The planner gives a rollout score out of 100 with a verdict, the waves with user counts and week ranges, the annual hours saved at full rollout, a review capacity check, the top 3 gaps with fixes, a phased plan, an effort estimate in person-days, and a printable checklist.

## How it works

- Three presets: a small team with a proven pilot, a department rollout, and a regulated rollout with gaps to close. Every field is editable, and Clear all resets the form.
- Scoring, stated on the page so you can disagree with it: pilot evidence 30 (hours proved 15, pilot users 15), data and guardrails 25 (sensitivity 9, data sources 8, four gates 8), review capacity 25 (one in five answers reviewed, capacity against need), training and change 20 (training hours 8, champions 7, announcement and support channel 5).
- Verdicts: 75 or more is Roll out now, 50 to 74 is Roll out in waves, below 50 is Fix the gaps first.
- Waves: wave 1 is the champions and pilot users, wave 2 is 40 percent of the rest, wave 3 is everyone else. Prep takes two weeks, wave 1 takes two, later waves take three or four weeks depending on team count and rollout size.
- Review capacity: one in five requests needs a human look. If the named reviewers cannot cover that many answers a day, the plan names the shortfall and the fix.
- Effort: 5 days of prep, 2 days per team, 1 day per data source, 2 days for confidential data or 4 for regulated data, plus training delivery at one trainer day per 16 user hours.

## Running it

Open `index.html` in any browser. It runs entirely in your browser. There is no server, no API key, no account, and nothing you enter leaves the page.

## Sources

Built from the Harness Readiness Check in Janaki's article "Harness Engineering: The Discipline That Separates Production AI Agents from Demos" (LinkedIn, 24 November 2026): the four gates in this planner are logging, a cost ceiling, a fallback on the third failed call, and scoped access. The step before this plan is the AI Pilot Planner, and the check before that is the AI Readiness Assessment. The running cost of the assistant is priced by the AI Cost Estimator. Scoring weights, the one in five review rate, and the wave sizes are planning rules from practice, not vendor numbers.

## What to do next

Email Janaki with your rollout size, your score, and your verdict, and she will tell you what to fix first. Or book a session and bring the plan.

# AI Agent Monitoring Dashboard

The pilot worked for five people. Then it went live, and nobody watched it.

Pick an assistant and a day range and this working single-file web app shows what watching looks like: total runs, success rate, grounded answers, average latency, cost, the worst day, a runs-per-day chart, health by assistant, the failed runs by cause with the fix for each, and the five most recent failed runs with the question that failed. Every number is computed live in your browser from the sample data.

## What it does

- **Three sample assistants, 30 days of runs each:** Permit Questions Assistant (document-grounded Q and A), Document Intake Assistant (extraction and classification), GIS Helpdesk Assistant (general Q and A).
- **Six live indicators:** total runs, success rate, grounded answers, average latency, total cost, and the worst day, all recomputed when you change the filters.
- **Health by assistant:** Healthy means success at 98 percent or better, grounded answers at 95 percent or better, and average latency under 3 seconds. Watch means success at 95 percent or better and grounded at 90 percent or better. Anything below that needs attention.
- **Runs-per-day chart:** green bars are ordinary days, amber bars are days with a failure rate above 5 percent, red bars are the two incident days, a rate-limit spike on the intake assistant and an ungrounded-answer spike on the helpdesk assistant.
- **Why runs failed:** five causes, each with the count, the share, and the fix that closes it.
- **Recent failed runs:** the five most recent failures with the date, the assistant, the question, and the cause.
- **What a production version adds:** real telemetry, alerts on thresholds, a cost ceiling that bites, groundedness checks on every answer, and access control and retention for run logs.

## Grounded in

- The harness gates and full logging from Janaki Gattu's article *Harness Engineering: The Discipline That Separates Working Agents from Expensive Demos* (LinkedIn, 24 Nov 2026).
- Cost thinking from the AI Cost Estimator on this portfolio, and monitoring patterns from the ArcGIS Monitor Deployment Planner and the ArcGIS Monitor guide.

The three assistants and their 30 days of runs are sample data, generated in the browser from fixed numbers so the dashboard is the same on every load. Thresholds, shares, and sample runs are planning rules from practice, not vendor numbers.

## How to run it

Open `index.html` in any browser. No backend, no API key, no account. Nothing you click is sent anywhere.

## Next step

Email Janaki with the assistant you run and the number that worries you most, success rate, cost, or grounded answers, and she will help you set up the monitoring that catches the next failure before a user reports it: gjanaki360@gmail.com. Or book a session at https://janakigattu.github.io/.

Janaki Gattu, Enterprise GIS Consultant. LinkedIn: https://www.linkedin.com/in/janaki-gis-enterprise

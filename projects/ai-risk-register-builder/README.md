# AI Risk Register Builder

The risk nobody writes down is the one that bites.

## What it does

Pick the risks that apply to your assistant from a list of ten, rate how likely each one is and how bad it would be, and get a scored risk register: every risk ranked by score, the top three to fix first with the mitigation and the named owner for each, a posture score out of 100 with a verdict (Ready to proceed, Proceed with controls, or Stop and fix first), and a printable register and checklist.

## How the score works

Risk score is likelihood times impact, from 1 to 25. Bands: 1 to 4 Low, 5 to 9 Medium, 10 to 15 High, 16 to 25 Critical. Posture starts at 100 and subtracts 12 per Critical risk, 7 per High, 3 per Medium, and 1 per Low, floored at 0. Verdict: 85 or higher Ready to proceed, 60 to 84 Proceed with controls, below 60 Stop and fix first. One Critical risk drops the verdict a full band, whatever the score says. All of those are planning rules from practice, not vendor numbers, and the page says so.

## Run it

Open `index.html` in a browser. No backend, no API key, no account, nothing sent or stored. Three presets show the range: a small team internal assistant (90, Ready to proceed), a public agency citizen facing assistant (50, Stop and fix first), and a GIS team document assistant (83, Proceed with controls). Print button included.

## Sources

The Harness Readiness Check from Janaki Gattu's article "Harness Engineering: The Discipline That Separates Real AI Agents from Demos" (LinkedIn, 24 Nov 2026). Next steps on this site: the AI Acceptable Use Policy Builder writes the rules the register enforces, the AI Agent Eval Harness tests the safety risks before the assistant ships, the AI Agent Monitoring Dashboard watches the risks once it is live, and the AI Agent Failure Review finds the cause when one of them happens.

## Talk to Janaki

Email gjanaki360@gmail.com with the top risk and the posture score, or book a session at janakigattu.github.io and work through the register together.

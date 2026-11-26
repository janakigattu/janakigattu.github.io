# AI Pilot Planner

Most AI pilots fail on the data and the guardrails, not the model. Plan the pilot before you build it, and judge it on one number.

## What it does

Pick one task your team repeats, say how many hours it takes, where the data lives, who checks the output, and what kind of data it touches. The planner returns a 30-day pilot plan: a readiness score out of 100, a verdict (Go, Go with guardrails, or Fix the data first), the gaps to close first, a week by week plan, the guardrails for this pilot, an effort estimate in person-days, and a printable checklist.

The plan follows the Harness Readiness Check from Janaki Gattu's article, Harness Engineering: The Discipline That Separates Production AI Agents from Demos. Week 1 covers gates 1 and 2 (every tool and data source listed, write access scoped to the task). Week 2 covers gates 3 to 6 (fallback on the third failed call, isolated execution, cost ceiling, full logging). Week 4 judges the pilot on one number: the hours saved per week the user set at the start.

## How to run it

Open `index.html` in any browser. No backend, no API key, nothing you type leaves the page. Three presets fill the form: small team document intake, email triage, and report drafting on regulated data. The Print button prints the plan and checklist.

## Scoring

Readiness is data readiness (30), a named reviewer (25), data sensitivity handling (25), and hours at stake (20). 75 and above is Go, 50 to 74 is Go with guardrails, below 50 is Fix the data first. The success number is the hours saved per week you set; the annual figure is that number times 48 working weeks.

## Sources

Janaki Gattu, Harness Engineering: The Discipline That Separates Production AI Agents from Demos, LinkedIn, 24 Nov 2026. https://www.linkedin.com/pulse/harness-engineering-discipline-separates-production-ai-janaki-gattu-jdcdc/

## What to do next

Email Janaki the use case and your success number, and she will tell you honestly whether the pilot is worth running: gjanaki360@gmail.com. Or book a session at https://janakigattu.github.io/#book and work through the plan together in one conversation.

# AI Agent Eval Harness

A pilot that impresses five people can still fail the sixth question. This harness runs twelve tests against a sample assistant and grades it, so you find the failures before your users do.

## What it does

Pick one of three sample assistants and run the eval. Twelve tests across four categories: Groundedness, Accuracy, Safety, and Cost and speed. Every test compares the assistant's answer against the expected facts, the forbidden words, or a numeric limit, and the score is computed live in your browser.

- **Grounded Assistant**: answers only from the documents, cites the section, refuses what is off limits. Slow on long questions. Scores 92 out of 100. Ship it.
- **Confident Assistant**: answers fast and sounds certain, but invents numbers and skips the conditions. Scores 42 out of 100. Do not ship.
- **Loose Assistant**: answers from the documents, but shares what it should refuse and costs more per run. Scores 75 out of 100. Fix the failures first.

The results show the score by category, all twelve tests with the expected facts, the answer given, and why each test passed or failed, plus the failed tests with the fix for each.

## How it works

No backend, no API key, no account. Open `index.html` in a browser. The three assistants and their answers are sample data, built to show three different failure modes. The checks are real: text tests pass only when the answer contains every required fact and none of the forbidden words; number tests pass only when the measured value stays inside the limit. A production version runs your own test set against your own assistant.

## Sources

- The harness thinking comes from Janaki Gattu's article, Harness Engineering: The Discipline That Separates Production AI from Expensive Demos: https://www.linkedin.com/pulse/harness-engineering-discipline-separates-production-ai-janaki-gattu-jdcdc/
- Version facts from the ArcGIS Enterprise Upgrade Planner on this portfolio; credit rates from the ArcGIS Online Credit Estimator.
- Scoring weights and thresholds are planning rules from practice, not vendor numbers.

## Live demo

https://janakigattu.github.io/projects/ai-agent-eval-harness/

## Next step

Email Janaki with the assistant you want graded, the test set it has to pass, and the score it has to reach before it ships: gjanaki360@gmail.com. Or book a session at https://janakigattu.github.io/.

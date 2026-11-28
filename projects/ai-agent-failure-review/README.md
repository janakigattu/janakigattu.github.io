# AI Agent Failure Review

The wrong answer is already out. The question now is why it happened, what fixes it, and how you prove the fix before the assistant goes back live.

## What it does

Pick a failure type and answer six short questions, and the review names the severity, the most likely root cause with the reasoning in plain language, the fix mapped to the harness gate it belongs to, a retest set of five concrete checks that must all pass before the assistant goes back live, and a prevention checklist.

- **Seven failure types**: invented fact, ungrounded answer from the wrong document, refused a valid question, slow or timed out, cost spike, restricted content leaked, tool call failed.
- **Six questions**: which assistant, reproducible or one-off, how many users saw it, logs available, which document set it answers from, when it happened.
- **Three severities**: Stop it now, Fix before the next release, Watch it. A leaked restriction that many users saw and that repeats is Stop it now. A one-off slow answer seen by one user, with full logs, is Watch it.
- **Three presets**: Ungrounded answer in production (Stop it now), Invented citation (Fix before the next release), Cost spike overnight (Watch it). Plus Clear all and a Print button for the review.

The results show how the score was built, factor by factor, so the severity is never a black box. The retest set is a tickable checklist: the assistant goes back live only when all five checks pass.

## How it works

No backend, no API key, no account. Open `index.html` in a browser. The severity score is computed live from the six answers: the failure type sets the base, reproducibility, users affected, logs, timing, and document set add points. The bands are 50 and above for Stop it now, 30 and above for Fix before the next release, below 30 for Watch it. Every failure type carries its own root cause, reasoning, fix, and five retest checks. Nothing typed is sent or stored anywhere.

## Sources

- The six harness gates come from Janaki Gattu's article, Harness Engineering: The Discipline That Separates Production AI from Expensive Demos: https://www.linkedin.com/pulse/harness-engineering-discipline-separates-production-ai-janaki-gattu-jdcdc/
- The failure causes match the AI Agent Monitoring Dashboard on this portfolio; the retest checks reuse the twelve tests from the AI Agent Eval Harness.
- Severity bands, scoring weights, and sample incidents are planning rules from practice, not vendor numbers.

## Live demo

https://janakigattu.github.io/projects/ai-agent-failure-review/

## Next step

Email Janaki with the failure type, the root cause, and the severity: gjanaki360@gmail.com. Or book a session at https://janakigattu.github.io/.

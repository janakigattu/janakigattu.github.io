# AI Acceptable Use Policy Builder

The cheapest AI policy is the one written before the first incident, not after it.

Answer seven questions about your team, and this working single-file web app writes a tailored AI acceptable-use policy you can copy, print, and adopt. It also gives you a completeness score out of 100 and names the gaps to close before the policy is ready.

## What it does

- **Three presets:** Small business, Public agency, GIS team, or fill in your own answers.
- **Seven inputs:** organisation name and type, approved AI tools, allowed uses, what must never go into an AI tool, the human review rule, a named policy owner, and a next review date, plus a logging rule.
- **Completeness score out of 100:** tools 15, uses 15, off-limits categories 25, human review 20, owner 15, logging 10. Verdict: Ready to adopt at 75 or above, Usable with gaps at 50 to 74, Not ready yet below 50.
- **A real policy document:** seven numbered sections (Purpose, Approved tools, What AI may be used for, What must never go into an AI tool, Human review, Logging, Ownership and review) rendered as a clean printable document, with Copy and Print buttons.
- **Gaps with fixes:** every missing piece is named with the fix that closes it.

## Grounded in

- The Harness Readiness Check from Janaki Gattu's article *Harness Engineering: The Discipline That Separates Working Agents from Expensive Demos* (LinkedIn, 24 Nov 2026): a human in charge, scoped write access, a fallback when a call fails, isolated execution, a cost ceiling, and full logging. The policy turns those guardrails into rules a team can follow.
- ArcGIS AI Assistants availability follows Esri's *What's new in AI assistants, June 2026*.

Scoring weights and the policy wording are planning rules from practice, not vendor numbers. The policy is a starting draft, not legal advice: have your own counsel review it before you adopt it.

## How to run it

Open `index.html` in any browser. No backend, no API key, no account. Nothing you type is sent anywhere.

## Next step

Email Janaki with your organisation type and your completeness score, and she will help you turn the draft into a policy your team actually follows: gjanaki360@gmail.com. Or book a session at https://janakigattu.github.io/.

Janaki Gattu, Enterprise GIS Consultant. LinkedIn: https://www.linkedin.com/in/janaki-gis-enterprise

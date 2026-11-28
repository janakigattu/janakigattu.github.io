# AI Model Picker for GIS Teams

The strongest model is not always the right model. Pick the task, say how accurate it must be, how fast it must answer, and how sensitive the data is, and this picker names the cheapest tier that does the job properly, with the monthly cost to prove it.

## What it does

Pick one of six tasks and answer three questions, and the picker names the recommended model tier (Lightweight, Balanced, or Flagship), the monthly model cost for that tier, a comparison table pricing all three tiers on the same volume, the reasoning behind the pick, and the privacy rule for the data sensitivity you chose.

- **Six tasks**: drafting documents, summarising long documents, writing ArcGIS code, analysing images and maps, translating text, extracting structured data. Drafting and translation start at Lightweight; the other four start at Balanced.
- **Three questions**: how accurate it must be (nice to have / important / must be right every time), how fast it must answer (seconds / a minute / batch overnight), how sensitive the data is (public / internal / confidential / regulated).
- **Three tiers**: Lightweight (Gemini 2.5 Flash, $0.30 in / $2.50 out per 1M tokens), Balanced (GPT-5, $1.25 / $10.00), Flagship (Claude Sonnet 4.5, $3.00 / $15.00). Rates checked 26 Nov 2026.
- **Three presets**: Quick internal drafting (Lightweight, $1.02/month), Regulated document summaries (Flagship, $10.80/month), Map image analysis at scale (Balanced, $11.00/month). Plus Clear all and a Print button for the recommendation.

The pick is never a black box: every reason is listed, including when accuracy and speed pull in opposite directions. Data sensitivity never changes the model pick; it changes how the data reaches the model.

## How it works

No backend, no API key, no account. Open `index.html` in a browser. The tier starts from the task, moves up one tier when the answer must be right every time, and moves down one tier when seconds matter. The monthly cost is conversations times input and output tokens times the published per-token rate. Nothing typed is sent or stored anywhere.

## Sources

- Model rates checked 26 Nov 2026 on the OpenAI, Anthropic, and Google pricing pages.
- The AI Cost Estimator on this portfolio prices the full running cost, including human review and hosting.
- Tier rules, task bases, and the privacy guidance are planning rules from practice, not vendor numbers.

## Live demo

https://janakigattu.github.io/projects/ai-model-picker-for-gis-teams/

## Next step

Email Janaki with the task, the tier this picker recommended, and the monthly cost: gjanaki360@gmail.com. Or book a session at https://janakigattu.github.io/.

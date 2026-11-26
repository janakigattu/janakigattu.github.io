# AI Cost Estimator

The pilot was cheap. The running bill is the surprise. Price the month before you commit to it.

## What it does

Enter how much your AI assistant will actually be used, and this estimator prices the month: the model cost at your provider's rates, the human review cost, and the fixed hosting cost. It names the biggest cost driver, gives the two fixes that cut the bill fastest, and shows what the same usage costs on the other two model tiers.

## How it works

- Three presets: a small team internal assistant, a customer support assistant, and a document-heavy assistant. Every number is editable.
- Three model tiers with editable prices, starting from the providers' published list prices checked 26 November 2026: Lightweight (Gemini 2.5 Flash rates: $0.30 in, $2.50 out, $0.03 cached per 1M tokens), Balanced (GPT-5 rates: $1.25 in, $10.00 out, $0.125 cached), Flagship (Claude Sonnet 4.5 rates: $3.00 in, $15.00 out, $0.30 cached).
- Human review is priced as a line item, because in most pilots it costs more than the model. Reviews per day, minutes per review, and the reviewer's loaded hourly cost.
- Output: monthly total, annual projection, cost per conversation, a line-item table with the biggest driver flagged, a same-usage comparison across all three tiers, and a print button.
- Verdicts: under $100 a month is small pilot money, $100 to $999 is a real monthly line item, $1,000 to $4,999 is a budget line worth owning, $5,000 and up is board-level money.

## Running it

Open `index.html` in any browser. It runs entirely in your browser. There is no server, no API key, no account, and nothing you enter leaves the page.

## Sources

Model prices checked 26 November 2026 from the providers' own pricing pages: OpenAI pricing, Anthropic pricing, and Gemini API pricing. Prices move and models retire, so confirm your model's current rates before you build a budget on this. The review and hosting numbers are yours to set, not ours to guess.

## What to do next

Email Janaki with your monthly total and your biggest cost driver, and she will tell you what to change first. Or book a session at janakigattu.github.io and bring the numbers from this page.

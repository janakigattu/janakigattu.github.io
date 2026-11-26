# Document-Grounded AI Assistant

An AI assistant is only as trustworthy as the documents it answers from. Ask a question and watch it answer from the documents, with the source shown for every line.

## What it does

A working retrieval demo, built by Janaki Gattu. It answers questions from three sample document sets, eighteen passages in total:

- **City of Riverton GIS Data Sharing Policy** (sample): what may be published openly, what stays internal, how often each dataset is updated, and how outside requests are handled.
- **ArcGIS Enterprise 11.5 Upgrade Checklist** (sample, from Esri's published guidance): backup, component order, direct upgrades, scene layer caches, and the rollback that exists when there is no downgrade.
- **Enterprise GIS Support Services, Sample RFP Scope** (sample): response times, monitoring, patching, reporting, working hours, and documentation.

Ask a question in your own words, or tap one of the six suggested questions. The demo:

- Matches your question against the passages and retrieves the best ones
- Builds the answer only from the retrieved passages, nothing invented
- Shows the source document and section for every line, with a relevance score
- Lists the words it matched, so you can see why it picked those passages
- Says plainly when no document covers your question, instead of guessing

You can also read all eighteen passages in full, from the "Read all eighteen passages" toggle.

## How to run it

Open `index.html` in a browser. That is all. It runs entirely in your browser: no server, no backend, no API key, no account, and nothing you type leaves the page. The retrieval runs on your device and nothing is stored or sent anywhere.

## What it is built from

The upgrade facts come from Esri's published documentation: the ArcGIS Enterprise upgrade order, the direct upgrade table, the hosted scene layer cache migration at 11.5, and WebGISDR backup and restore. The data sharing policy and the RFP scope are samples written for this demo. Riverton is a fictional city, and the scope is not a real contract. The retrieval pattern follows Janaki Gattu's article [Harness Engineering: the discipline that separates production AI agents from demos](https://www.linkedin.com/pulse/harness-engineering-discipline-separates-production-ai-janaki-gattu-jdcdc/).

## What to do next

Email Janaki at [gjanaki360@gmail.com](mailto:gjanaki360@gmail.com) with the document set you would ground an assistant on, or [book a session](https://janakigattu.github.io/#book) and bring the three documents your team asks about most. This demo answers from samples. A production version connects to your team's real documents.

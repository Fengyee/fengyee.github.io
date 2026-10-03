---
title: 'A Topology-Guided GeoAI Agentic Framework for Urban Flood Screening'
authors:
  - Yutian Tao
  - Haoan Feng
  - Xin Xu
  - Leila De Floriani
highlight_name: true
date: '2026-11-03'
publishDate: '2026-10-03'
publication_types:
  - paper-conference
publication: 'In *The 1st ACM SIGSPATIAL Student Challenge on Open Agents with Spatial Intelligence for Social Good (OASIS 2026)*, to appear'
publication_short: 'In *ACM SIGSPATIAL 2026 Workshop / Student Challenge (OASIS)*, to appear'
abstract: "Open-world geographic artificial intelligence (GeoAI) agents can transform public geospatial data into accessible decision support for real-world challenges, but must balance autonomous reasoning with reliable spatial analysis and human oversight. We present a topology-guided GeoAI agentic framework for urban flood screening that takes a place name, drawn region, or uploaded boundary and returns ranked candidate basins with an interactive map and report. A deterministic controller retrieves public elevation, rainfall, soil, land-cover, exposure, and infrastructure layers, extracts terrain depressions with discrete Morse theory, and ranks basins with a relative flood-priority score. The language model acts only at recorded decision points: selecting a persistence threshold from a precomputed candidate table, drafting recommendations from computed evidence, and reviewing each recommendation against the same evidence. Three human-in-the-loop checkpoints let users revise the threshold, factor weights, or recommendation. In a College Park, Maryland case study, the selected threshold reduced 278 raw terrain minima to 70 basins, with 77% of these basins' lowest points also identified as sinks by a separately computed eight-direction (D8) flow-routing model. Across four further study areas, agreement ranged from 61% to 83%. By combining open data, explicit spatial reasoning, traceable evidence, and human oversight, the framework enables transparent first-pass flood screening while keeping consequential recommendations inspectable and user-controlled."
summary: 'A topology-guided GeoAI agentic framework combining public geospatial data, deterministic terrain analysis, evidence-grounded LLM decisions, and human oversight for urban flood screening. Top-10 finalist at OASIS 2026.'
tags:
  - GeoAI
  - Spatial Intelligence
  - Topological Data Analysis
  - Human-in-the-Loop
  - Urban Flood Screening
featured: false
links:
  - name: OASIS 2026
    url: 'https://rsvp.withgoogle.com/events/oasis-2026/'
---

{{% callout note %}}
**Accepted at OASIS 2026**, the ACM SIGSPATIAL Student Challenge on Open Agents with Spatial Intelligence for Social Good. Our team is a **top-10 finalist** and was selected for an **on-site presentation and demo** in Riverside, CA, on November 3, 2026.

Our team received a **Google DeepMind Student Travel Grant** to support participation.
{{% /callout %}}

{{< figure src="figure-1.png" link="figure-1.png" target="_blank" rel="noopener" alt="Five-stage workflow showing data acquisition, topological analysis, ranking and validation, recommendation and reflection, and interactive outputs. Purple arrows mark three human-in-the-loop checkpoints." caption="Figure 1. Workflow of the framework with intermediate results. Deterministic stages retrieve and align data, extract and rank Morse basins, and compare them with D8 routing and with re-ranking under alternative weights. Separate language-model calls select the persistence threshold, draft the recommendation, review it against the recorded evidence, and answer later user questions. Purple arrows mark the three human-in-the-loop (HITL) checkpoints." >}}

The framework starts from a place name or boundary, retrieves public geospatial layers, extracts terrain basins using discrete Morse theory, and ranks them for preliminary flood screening. Language-model calls select a persistence threshold, draft recommendations, and review them against the computed evidence. Three human checkpoints allow users to revise the threshold, ranking weights, or recommendation.

The evaluation covers five study areas. It measures agreement with D8 flow routing on the same elevation grid and checks ranking sensitivity; the scores support preliminary screening and are not calibrated flood probabilities.

The paper is not yet available on arXiv. The assigned DOI is `10.1145/3849739.3856761`; its landing page is not yet available.

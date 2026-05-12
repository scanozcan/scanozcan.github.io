---
layout: post
title: "GLproxScape: Spatial Deconvolution of dCas9-APEX2 Proximity Proteomics"
date: 2026-05-12
categories: news
published: false
---

I have been developing [GLproxScape](https://github.com/scanozcan/GLproxScape), an R package that performs spatial deconvolution of **dCas9-APEX2 proximity proteomics** data into transcription-factor and chromatin-regulator binding predictions. The package models each guide RNA's biotinylation footprint as a Gaussian labelling cone (default σ = 300 bp), forward-smears per-region proteomics enrichment into a continuous spatial track *s(x)*, and normalises by guide coverage *C(x)* to recover a promoter-wide occupancy estimate β(x). Binding events are then deconvolved on a [JASPAR](https://jaspar.elixir.lu) position-weight-matrix basis. A separate zone-based path handles chromatin readers, writers, erasers, and remodellers that lack a sequence-specific motif (e.g. BRD4, KMT2A, SMARCA4), and an optional [ChIP-Atlas](https://chip-atlas.org) overlay validates predictions against independent ChIP-seq peaks. The first version has now been uploaded to [GitHub](https://github.com/scanozcan/GLproxScape), along with a bundled reanalysis of the Mackenzie 2026 FOXP2 dataset as an end-to-end example.

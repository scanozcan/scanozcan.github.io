---
layout: post
title: "GLproxScape: Spatial deconvolution of genomic locus proteomics"
date: 2026-05-12
categories: news
published: true
github: "https://github.com/scanozcan/GLproxScape"
---

<div style="text-align:center; margin-bottom:1.5rem;">
  <img class="theme-logo-light" src="/assets/images/GLproxScape-light.svg" alt="GLproxScape logo" style="max-width:360px; width:100%;">
  <img class="theme-logo-dark"  src="/assets/images/GLproxScape-dark.svg"  alt="GLproxScape logo" style="max-width:360px; width:100%;">
</div>

[GLproxScape](https://github.com/scanozcan/GLproxScape) is an R package that performs spatial deconvolution of **genomic locus proteomics** data into transcription-factor and chromatin-regulator binding predictions. The package models each region's biotinylation footprint as a Gaussian labelling cone (default σ = 300 bp), forward-smears per-region proteomics enrichment into a continuous spatial track *s(x)*, and normalizes by guide coverage *C(x)* to recover a genomic locus-wide occupancy estimate β(x). Binding events are then deconvolved on a [JASPAR](https://jaspar.elixir.lu) position-weight-matrix basis. A separate zone-based path handles chromatin readers, writers, erasers, and remodellers that lack a sequence-specific motif, and an optional [ChIP-Atlas](https://chip-atlas.org) overlay validates predictions against independent ChIP-seq peaks. The first version has now been uploaded to GitHub, along with a bundled reanalysis of the Mackenzie 2026 FOXP2 dataset as an end-to-end example.

<div style="text-align:center;">
  <img src="/assets/images/glproxscape-example.png" alt="GLproxScape binding event deconvolution example — MAZ and ZXDC promoter occupancy profiles" style="max-width:100%;">
</div>

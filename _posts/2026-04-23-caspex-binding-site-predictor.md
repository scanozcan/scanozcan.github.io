---
layout: post
title: "New tool: CasPEX Binding Zone Predictor"
date: 2026-04-23
categories: news
---

I released [CasPEX Binding Zone Predictor](https://github.com/scanozcan/Caspex-binding-site-predictor), an R pipeline that reconstructs transcription factor binding locations from CasID proximity-labeling proteomics data. When multiple guide RNAs tile across a promoter, their APEX-labeling signals overlap and blur, making it difficult to pinpoint where a factor actually binds. The pipeline addresses this by projecting per-region logFC values onto a continuous promoter coordinate system, smoothing with a Gaussian kernel matched to the APEX labeling radius (~250 bp), normalizing for uneven guide RNA spacing, and decomposing the resulting landscape into discrete binding events anchored to TF motifs — producing spatial predictions at single-region resolution along with publication-quality diagnostic plots.

<img src="{{ '/assets/images/caspex-example-prediction.png' | relative_url }}" alt="Example CasPEX binding site prediction" style="width: 100%; max-width: 900px; display: block; margin: 20px auto;">

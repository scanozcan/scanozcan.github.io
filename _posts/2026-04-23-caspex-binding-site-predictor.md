---
layout: post
title: "CASPEX TF-Binding Zone Predictor"
date: 2026-04-23
categories: news
---

For a while, I have been working on [CASPEX TF-Binding Zone Predictor](https://github.com/scanozcan/Caspex-binding-site-predictor), an R pipeline that predicts the transcription factor binding locations from CASPEX (GloPro) proximity-labeling proteomics enrichment data. The pipeline projects per-region logFC values onto a continuous promoter coordinate system, smoothing with a Gaussian kernel matched to the APEX labeling radius (~250 bp), normalizing for uneven guide RNA spacing, and decomposing the resulting landscape into discrete binding events anchored to TF motifs. The first version has now been uploaded to [GitHub](https://github.com/scanozcan/Caspex-binding-site-predictor), along with an example dataset.

<img src="{{ '/assets/images/caspex-example-prediction.png' | relative_url }}" alt="Example CasPEX binding site prediction" style="width: 100%; max-width: 900px; display: block; margin: 20px auto;">

<img src="{{ '/assets/images/caspex-example-prediction-2.png' | relative_url }}" alt="Example CasPEX binding site prediction" style="width: 100%; max-width: 900px; display: block; margin: 20px auto;">

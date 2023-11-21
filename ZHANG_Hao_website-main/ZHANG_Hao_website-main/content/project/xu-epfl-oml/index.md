---
title: The effect of delay and momentum in Asynchronous Stochastic Gradient Descent
summary: Course Project for EPFL Optimization for Machine Learning
tags:
  - Deep Learning
date: '2022-06-12T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Test Accurancy with different delay 
  focal_point: Smart

links:
  # - icon: twitter
    # icon_pack: fab
    # name: Follow
    # url: https://twitter.com/georgecushen

url_code: 'https://github.com/BillyXYB/EPFL_OptML_Course'
url_pdf: files/CS_439_Report.pdf
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Training large machine learning models on large datasets is notoriously computationally heavy. When multiple workers are available, a common algorithm to perform the training is Asynchronous Stochastic Gradient Descent (ASGD), wherein gradients of the loss on mini-batches are computed by workers and added to the model weights by the server. The workers are not fully synchronized with the server, which enables speedup by parallelization. However, this asynchronicity causes the gradients to be computed with a “delay” compared to the actual model on the server. In this work, we simulate a simple version of ASGD allowing us to study the effect of delay only. Based on experiments on real-life data, we draw the following insights on the behavior of ASGD. We confirm the adverse effect of delay on the training process. We observe that past a certain threshold, delay may prevent training entirely. For large delays, using momentum improves the performance of ASGD dramatically.
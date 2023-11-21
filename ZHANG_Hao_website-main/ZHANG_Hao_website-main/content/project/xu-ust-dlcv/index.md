---
title: "LongStoryGAN: A Chronological Illustration Generation Framework For
Documents"
summary: Course Project for HKUST Deep Learning for Computer Vision
tags:
  - Deep Learning
date: '2020-06-10T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Results of LongStoryGAN
  focal_point: Smart

links:
  # - icon: twitter
    # icon_pack: fab
    # name: Follow
    # url: https://twitter.com/georgecushen

url_code: ''
url_pdf: files/COMP4471Proj.pdf
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Story visualization is a newly proposed task that com- bines computer vision with natural language processing. While neural image generation methods have enabled story visualization from image descriptions in previous works, they are not well suited to general text documents. To close this gap, we present a chronological illustration genera- tion framework, LongStoryGAN, which expands the input of story visualization to general documents. Our framework contains two major modules: the text summarization mod- ule and the image generation module. The text summariza- tion module applies the TextRank algorithm [8] to extract sentences in chronological order that contain the action of character. The image generation module is based on a modified state-of-the-art model on story visualization, Sto- ryGAN [7], which generates a series of images describing these sentences. Extensive experiments show that LongSto- ryGAN is able to illustrate a relatively long story using im- ages. In particular, we compare both modules with their individual ablations on corresponding datasets. Both qual- itative and quantitative results show that our modules out- perform their own ablation.  
---
title: High precision binary object detector Project
summary: High precision binary object detector based on BSF-XNOR CNN layer
tags:
- CNN
- Deep Learning
date: "2020-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by Huan Jiang
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

Although the binary network has a fast inference speed, it cannot be used directly on mobile devices such as unmanned Aerial Vehicle because of its low detection accuracy.
Different from improving the detection accuracy of the binary network by adjusting the network structure or adjusting the update gradient, we propose an improved binary neural network based on block scaling factor XNOR (BSFXNOR) convolution layer.
In addition, we propose a two-level densely connected network structure, which further enhances the feature representation capabilities of the network layer.
Our experiments prove the effectiveness of our algorithm in improving accuracy, compared with the original XNOR network, the mAP (mean Average Accuracy) detected by our algorithm on the PASCAL VOC2007 dataset has been improved from 48.2 to 62.4. 
Our algorithm provides guidance for deploying highprecision binary networks on heterogeneous parallel processors such as FPGAs, and solves the problem of low precision of binary networks.





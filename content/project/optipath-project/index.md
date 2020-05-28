---
title: Fast Three-Dimensional Path Planning with Obstacle Avoidance Constraints
summary: Path Planning Using Convex Optimization
tags:
- Path Planning
- Convex Optimization
date: "2020-01-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by Huan Jiang
  focal_point: Smart

links:
- icon: researchgate
  icon_pack: fab
  name: Follow
  url: https://researchgate.com/jianghuan7
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

This project addresses the three-dimensional path planning problem of unmanned aerial vehicles with obstacle avoidance constraints and an objective of minimizing the time of flight.
Solving this optimal control problem in real time for autonomous flight is very challenging.
The contribution of this paper is to convexify such a nonconvex and highly nonlinear problem into the framework of second-order cone programming (SOCP), which is a subclass of convex optimization and can be very efficiently solved by existing interior point methods. 
The convexification is novel in that almost no nonlinearity in the original problem is lost. 
This is very helpful for rapid convergence of the successive SOCP used to get the optimal solution of the original problem. 
Numerical examples are provided to show the validity and high efficiency of the proposed method for potential real-time path planning.





---
title: "Fast Three-Dimensional Path Planning with Obstacle Avoidance Constraints"
authors:
- Huan Jiang
- Xinfu Liu
date: "2019-01-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2019-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In AIAA Scitech 2019 Forum
publication_short: In AIAAScitechForum2019

abstract: This paper addresses the three-dimensional path planning problem of unmanned aerial vehicles with obstacle avoidance constraints and an objective of minimizing the time of flight. Solving this optimal control problem in real time for autonomous flight is very challenging. The contribution of this paper is to convexify such a nonconvex and highly nonlinear problem into the framework of second-order cone programming (SOCP), which is a subclass of convex optimization and can be very efficiently solved by existing interior point methods. The convexification is novel in that almost no nonlinearity in the original problem is lost. This is very helpful for rapid convergence of the successive SOCP used to get the optimal solution of the original problem. Numerical examples are provided to show the validity and high efficiency of the proposed method for potential real-time path planning.

# Summary. An optional shortened abstract.
summary: This paper addresses the three-dimensional path planning problem of unmanned aerial vehicles with obstacle avoidance constraints and an objective of minimizing the time of flight.

tags:
- Path Planning
- Convex Optimization
featured: true

links:
- name: Custom Link
  url: http://arc.aiaa.org/doi/abs/10.2514/6.2019-0357 
url_pdf: https://arc.aiaa.org/doi/abs/10.2514/6.2019-0357 
url_code: 'https://github.com/Algorhi'
url_dataset: '#'
url_poster: '#'
url_project: ''
url_slides: ''
url_source: '#'
url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [Huan](https://askyspace.com)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- optipath-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

{{% alert note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /alert %}}

{{% alert note %}}
Click the *Slides* button above to demo Academic's Markdown slides feature.
{{% /alert %}}

Supplementary notes can be added here, including [code and math](https://sourcethemes.com/academic/docs/writing-markdown-latex/).


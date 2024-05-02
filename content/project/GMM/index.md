---
title: "Learning a Mixture of Gaussians via Mixed-Integer Optimization"
authors:
- admin
date: "2022-03-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2022-03-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: We consider the problem of estimating the parameters of a multivariate Gaussian mixture model (GMM) given access to n samples that are believed to have come from a mixture of multiple subpopulations. State-of-the-art algorithms used to recover these parameters use heuristics to either maximize the log-likelihood of the sample or try to fit first few moments of the GMM to the sample moments. In contrast, we present here a novel mixed-integer optimization (MIO) formulation that optimally recovers the parameters of the GMM by minimizing a discrepancy measure (either the Kolmogorov–Smirnov or the total variation distance) between the empirical distribution function and the distribution function of the GMM whenever the mixture component weights are known. We also present an algorithm for multidimensional data that optimally recovers corresponding means and covariance matrices. We show that the MIO approaches are practically solvable for data sets with n in the tens of thousands in minutes and achieve an average improvement of 60%–70% and 50%–60% on mean absolute percentage error in estimating the means and the covariance matrices, respectively, over the expectation–maximization (EM) algorithm independent of the sample size n. As the separation of the Gaussians decreases and, correspondingly, the problem becomes more difficult, the edge in performance in favor of the MIO methods widens. Finally, we also show that the MIO methods outperform the EM algorithm with an average improvement of 4%–5% on the out-of-sample accuracy for real-world data sets.

# Summary. An optional shortened abstract.
summary: The paper introduces a novel approach for estimating parameters in a multivariate Gaussian mixture model (GMM). Instead of heuristic methods, the proposed mixed-integer optimization (MIO) formulation minimizes the discrepancy between empirical and GMM distribution functions. The MIO methods achieve significant improvements in parameter estimation accuracy compared to the expectation-maximization (EM) algorithm, especially as the separation between Gaussians decreases.

tags:
- Source Themes
featured: false

links:
# - name: Custom Link
#   url: https://pubsonline.informs.org/doi/abs/10.1287/ijoo.2018.0009
url_pdf: https://pubsonline.informs.org/doi/pdf/10.1287/ijoo.2018.0009
# url_code: ''
# url_dataset: '#'
# url_poster: '#'
# url_project: ''
# url_slides: ''
# url_source: '#'
# url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).

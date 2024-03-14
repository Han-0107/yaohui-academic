---
title: 'PUWR-TSSG: A CMAB Based Post-Unknown Worker Recruitment Scheme for Three-Stage Stackelberg Game in MCS'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jianheng Tang
  - Yaohui Han
  - Anfeng Liu*

# # Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2024-01-29T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: ''

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
# publication_types: ['Journal']

# Publication name and optional abbreviated publication name.
publication: Information Science (Submitted to Journal)
publication_short: INS

# abstract: Submitted to Journal

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: 'https://github.com/Han-0107/mcspy'
url_dataset: 'https://www.kaggle.com/datasets/chicago/chicago-taxi-trips-bq'
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---
## Abstract

Many three-stage Stackelberg game models have been proposed to describe the game process among task requesters, platforms, and workers for Mobile Crowd Sourcing  (MCS). These studies all assume that the platform knows the qualities of workers in advance or after receiving workers' data.  However, in reality, even after receiving workers' submitted data, the qualities of workers remain unknown, which is called the Post-Unknown Quality (PUQ) problem. Due to the PUQ  problem, the platform needs to expend considerable effort to identify worker quality in order to recruit high-quality workers and increase its own utilities. In such scenarios, the three-stage  Stackelberg game models used in previous studies, which assume the platform can identify worker qualities at zero cost,  cannot be applied to real-world MCS. In this paper, first, a  Double-level Truth Quality (DTQ) discovery approach is proposed to solve the PUQ problem for workers by employing bipartite-graph-based matrix completion technology in spatiotemporal MCS. Second, a Combinatorial Multi-Armed  Bandit (CMAB) based worker recruitment scheme is proposed by integrating the DTQ discovery approach, and the Upper  Confidence Bound (UCB) index is redesigned to include worker credibility to solve the exploration-exploitation dilemma, thus enabling recruitment of high-quality workers. Third, we model the payment computation problem as a three-stage Stackelberg game among three participants considering the PUQ problem,  in which the platform needs to pay a cost to verify workers,  which has not been considered in previous studies. We theoretically analyze the existence of a Stackelberg equilibrium at which no party has incentive to unilaterally deviate from its optimal strategy. We derive the optimal strategy group so that each party can maximize its own utility. Fourth, we find that the accuracy and cost of the platform's truth quality discovery significantly impact the Stackelberg game equilibrium, so we propose a Truth Quality Traceback (TQT) mechanism to enable more accurate worker identification and truth discovery at lower cost with faster convergence. Finally, we conduct extensive simulations on a real dataset to validate the effectiveness of the proposed strategies. 
<!-- {{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->

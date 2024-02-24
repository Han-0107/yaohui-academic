---
title: "WASIM: A Word-level Abstract Symbolic Simulation Framework for Hardware Formal Verification"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Hongce Zhang


# Author notes (optional)

date: "2023-04-22T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-04-22T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In Tools and Algorithms for the Construction and Analysis of Systems
publication_short: In TACAS

abstract: 

# Summary. An optional shortened abstract.
summary: Hardware Formal Verification for Processors

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: 'https://github.com/fangwenji/tacas23-wasim.git'
url_slides: 'https://hkustgz-my.sharepoint.com/:b:/g/personal/wfang838_connect_hkust-gz_edu_cn/EXSNwAonsOBFmBw_OnyavugBFZSUgr069TndqLJLa4APnQ?e=84PrmP'
url_source: ''
url_video: 'https://hkustgz-my.sharepoint.com/:v:/g/personal/wfang838_connect_hkust-gz_edu_cn/ESwTeGSliQ1IrhNXjyTxC1kBwXxupQgP29sodPZ0rnm0Ug?e=c6ACZP'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

This paper demonstrates the design and usage of WASIM, a word-level abstract symbolic simulation framework with pluggable abstraction/refinement functions. WASIM is useful in the formal verification of functional properties on register-transfer level (RTL) hardware designs. Users can control the symbolic simulation process and tune the level of abstraction by interacting with WASIM through its Python API. WASIM can be used to directly check formal properties on symbolic traces or to extract useful fragments from symbolic representations to construct safe inductive invariants as a correctness certificate. We demonstrate the utility of WASIM on the verification of two pipelined hardware designs. WASIM and the case studies is available under open-source license at https://doi.org/10.5281/zenodo.7247147.
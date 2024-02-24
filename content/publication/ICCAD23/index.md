---
title: "MasterRTL: A Pre-Synthesis PPA Estimation Framework for Any RTL Design"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Yao Lu
- Shang Liu
- Qijun Zhang
- Ceyu Xu
- Lisa Wu Wills
- Hongce Zhang
- Zhiyao Xie


# Author notes (optional)

date: "2023-07-21T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-07-21T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In International Conference of Computer-Aided Design
publication_short: In ICCAD

abstract: 

# Summary. An optional shortened abstract.
summary: Pre-Synthesis PPA Estimation

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/abstract/document/10323951'
url_code: ''
url_dataset: ''
url_poster: 'https://hkustgz-my.sharepoint.com/:b:/g/personal/wfang838_connect_hkust-gz_edu_cn/EQbBN7ZC1JpMte7_4TMdsw4B7VQ0e2dD6uwuM68OD2V96A?e=uiJDJZ'
url_project: 'https://github.com/hkust-zhiyao/MasterRTL'
url_slides: 'https://hkustgz-my.sharepoint.com/:b:/g/personal/wfang838_connect_hkust-gz_edu_cn/Edx0_KG4SddGsuxPUj5fcPIBKZJGLimfyQ7mSa45Eghqrg?e=BPS0zI'
url_source: ''
url_video: ''

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
In modern VLSI design flow, the register-transfer level (RTL) stage is a critical point, where designers define precise design behavior with hardware description languages (HDLs) like Verilog. Since the RTL design is in the format of HDL code, the standard way to evaluate its quality requires time-consuming subsequent synthesis steps with EDA tools. This time-consuming process significantly impedes design optimization at the early RTL stage. Despite the emergence of some recent ML-based solutions, they fail to maintain high accuracy for any given RTL design. In this work, we propose an innovative pre-synthesis PPA estimation framework named MasterRTL. It first converts the HDL code to a new bit-level design representation named the simple operator graph (SOG). By only adopting single-bit simple operators, this SOG proves to be a general representation that unifies different design types and styles. The SOG is also more similar to the target gate-level netlist, reducing the gap between RTL representation and netlist. In addition to the new SOG representation, MasterRTL proposes new ML methods for the RTL-stage modeling of timing, power, and area separately. Compared with state-of-the-art solutions, the experiment on a comprehensive dataset with 90 different designs shows accuracy improvement by 0.33, 0.22, and 0.15 in correlation for total negative slack (TNS), worst negative slack (WNS), and power, respectively.
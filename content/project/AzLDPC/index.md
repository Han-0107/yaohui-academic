---
title: Implementation of LDPC codec based on FPGA deployment in QKD
summary: Supervised by Prof. Duan Huang at CSU. (Patent Number 202310808424X)
tags:
  - FPGA
date: '2022-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

In the QKD communication system, the two communication parties need to negotiate the key under the condition of long distance and low signal-to-noise ratio. Therefore, lower bit rates and longer code words must be selected to ensure effective communication between the two sides. At present, LDPC decoding algorithms are mainly divided into two categories: bit flipping (BF) based on checksum statistical iteration and belief propagation (BP) based on probability. The hardware structure of encoder can be divided into serial structure, partially parallel structure and fully parallel structure. Considering that the encoder needs to reduce the output delay, this paper adopts a fully parallel hardware structure under the condition of sufficient hardware resources. In our study, we chose a bit flip based on checksum statistical iteration to implement our design.

At the same time, the encoder and decoder modules are designed as a pipeline structure. Our design allows users to encode or decode more information in a certain amount of time. Therefore, our LDPC system can achieve better performance and faster processing speed of information. At the same time, the number of induced I/O ports is small, and most of the complex structure of our design is integrated inside the module, so that our design can be easily ported to more devices, and users do not need to fully understand the internal structure of our module. In addition, we designed a program to simulate real communication in order to better understand the reliability and stability of this encoding method. Based on our logic design, we do a lot of experiments to ensure the stability and correctness of the module. In addition, we have developed the upper computer software suitable for this design, by adjusting different parameters, to ensure that this design can play a normal role in different communication scenarios.

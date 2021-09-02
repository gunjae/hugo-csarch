---
title: "Warped-Preexecution: A GPU Pre-Execution Approach for Improving Latency Hiding"
authors:
- Keunsoo Kim
- Sangpil Lee
- Myung Kuk Yoon
- admin
- Won Woo Ro
- Murali Annavaram
date: "2016-03-16T00:00:00Z"
doi: "10.1109/HPCA.2016.7446062"

# Schedule page publish date (NOT publication's date).
publishDate: "2016-03-16T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*International Symposium on High Performance Computer Architecture*"
publication_short: "*HPCA '16*"

abstract: "This paper presents a pre-execution approach for improving GPU performance, called P-mode (pre-execution mode). GPUs utilize a number of concurrent threads for hiding processing delay of operations. However, certain long-latency operations such as off-chip memory accesses often take hundreds of cycles and hence leads to stalls even in the presence of thread concurrency and fast thread switching capability. It is unclear if adding more threads can improve latency tolerance due to increased memory contention. Further, adding more threads increases on-chip storage demands. Instead we propose that when a warp is stalled on a long-latency operation it enters P-mode. In P-mode, a warp continues to fetch and decode successive instructions to identify any independent instruction that is not on the long latency dependence chain. These independent instructions are then pre-executed. To tackle write-after-write and write-after-read hazards, during P-mode output values are written to renamed physical registers. We exploit the register file underutilization to re-purpose a few unused registers to store the P-mode results. When a warp is switched from P-mode to normal execution mode it reuses pre-executed results by reading the renamed registers. Any global load operation in P-mode is transformed into a pre-load which fetches data into the L1 cache to reduce future memory access penalties. Our evaluation results show 23% performance improvement for memory intensive applications, without negatively impacting other application categories."

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac #convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- GPU
- SIMT
- Scheduling
featured: true

links:
- name: Custom Link
  url: http://example.org
url_pdf: http://eprints.soton.ac.uk/352095/1/Cushen-IMV2013.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
#projects:
#- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides:
---

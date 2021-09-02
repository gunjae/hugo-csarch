---
title: "CTA-Aware Prefetching and Scheduling for GPU"
authors:
- admin
- Hyeran Jeon
- Zhenhong Liu
- Nam Sung Kim
- Murali Annavaram
date: "2018-05-25T00:00:00Z"
doi: "10.1109/IPDPS.2018.00024"

# Schedule page publish date (NOT publication's date).
publishDate: "2018-05-25T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE International Parallel and Distributed Processing Symposium*"
publication_short: "*IPDPS '18*"

abstract: "Albeit GPUs are supposed to be tolerant to long latency of data fetch operation, we observe that L1 cache misses occur in a bursty manner for many memory-intensive applications. This in turn leads to severe contentions in GPU memory hierarchy, and thus stalls execution pipeline for many cycles as all warps end up waiting for their memory requests to be serviced by L1 cache. To spread such bursty L1 cache misses, we propose CTA-Aware Prefetcher and Scheduler (CAPS) consisting of a thread group-aware prefetcher and a prefetch-aware warp scheduler for GPUs. GPU kernels group threads into cooperative thread arrays (CTAs). Each thread typically uses its thread index and its associated CTA index to identify the data that it operates on. The starting base address accessed by the first warp in a CTA is difficult to predict since that starting address is a complex function of thread index and CTA index and also depends on how the programmer distributes input data across CTAs. But threads within each CTA exhibit stride accesses. Hence, if the base address of each CTA can be computed early, it is possible to accurately predict prefetch addresses for threads within a CTA. To compute the base address of each CTA, a leading warp is used from each CTA. The leading warp is executed early by pairing it with warps from currently executing leading CTA. The warps in the leading CTA are used to compute the stride value. The stride value is then combined with base addresses computed from the leading warp of each CTA to prefetch the data for all the trailing warps in the trailing CTAs. CAPS allows prefetch requests to be issued sufficiently ahead of time before the demand requests, effectively reorganizing warp executions to quickly detect the base address of each CTA and stride per load. CAPS predicts addresses with over 97% accuracy and is able to improve GPU performance by 8% on average with up to 27% for a wide range of GPU applications."

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac #convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- GPU
- Prefetch
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

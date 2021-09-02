---
title: "Access Pattern-Aware Cache Management for Improving Data Utilization in GPU"
authors:
- admin
- Yunho Oh
- Won Woo Ro
- Murali Annavaram
date: "2017-06-24T00:00:00Z"
doi: "10.1145/3079856.3080239"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-06-24T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*International Symposium on Computer Architecture (ISCA)*"
publication_short: "*ISCA '17*"

abstract: "Long latency of memory operation is a prominent performance bottleneck in graphics processing units (GPUs). The small data cache that must be shared across dozens of warps (a collection of threads) creates significant cache contention and premature data eviction. Prior works have recognized this problem and proposed warp throttling which reduces the number of active warps contending for cache space. In this paper we discover that individual load instructions in a warp exhibit four different types of data locality behavior: (1) data brought by a warp load instruction is used only once, which is classified as streaming data (2) data brought by a warp load is reused multiple times within the same warp, called intra-warp locality (3) data brought by a warp is reused multiple times but across different warps, called inter-warp locality (4) and some data exhibit both a mix of intra- and inter-warp locality. Furthermore, each load instruction exhibits consistently the same locality type across all warps within a GPU kernel. Based on this discovery we argue that cache management must be done using per-load locality type information, rather than applying warp-wide cache management policies. We propose Access Pattern-aware Cache Management (APCM), which dynamically detects the locality type of each load instruction by monitoring the accesses from one exemplary warp. APCM then uses the detected locality type to selectively apply cache bypassing and cache pinning of data based on load locality characterization. Using an extensive set of simulations we show that APCM improves performance of GPUs by 34% for cache sensitive applications while saving 27% of energy consumption over baseline GPU."

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac #convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- GPU
- Cache
- Access Pattern
featured: true

links:
- name: Slide Show
  url: https://filedn.com/luEeJVCCazShDlU4ibloXvu/publication/gpu_apcm_isca17/gpu_apcm_isca17_slides.ppsx
url_pdf: https://filedn.com/luEeJVCCazShDlU4ibloXvu/publication/gpu_apcm_isca17/gpu_apcm_isca17.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: https://filedn.com/luEeJVCCazShDlU4ibloXvu/publication/gpu_apcm_isca17/gpu_apcm_isca17_slides.pdf
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  caption: 'A cache management scheme of APCM'
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

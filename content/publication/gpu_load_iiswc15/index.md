---
title: "Revealing Critical Loads and Hidden Data Locality in GPGPU Applications"
authors:
- admin
- Hyeran Jeon
- Murali Annavaram
date: "2015-10-06T00:00:00Z"
doi: "10.1109/IISWC.2015.23"

# Schedule page publish date (NOT publication's date).
publishDate: "2015-10-06T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE International Parallel and Distributed Processing Symposium*"
publication_short: "*IPDPS '18*"

abstract: "In graphics processing units (GPUs), memory access latency is one of the most critical performance hurdles. Several warp schedulers and memory prefetching algorithms have been proposed to avoid the long memory access latency. Prior application characterization studies shed light on the interaction between applications, GPU micro architecture and memory subsystem behavior. Most of these studies, however, only present aggregate statistics on how memory system behaves over the entire application run. In particular, they do not consider how individual load instructions in a program contribute to the aggregate memory system behavior. The analysis presented in this paper shows that there are two distinct classes of load instructions, categorized as deterministic and non-deterministic loads. Using a combination of profiling data from a real GPU card and cycle accurate simulation data we show that there is a significant performance impact disparity when executing these two types of loads. We discuss and suggest several approaches to treat these two load categories differently within the GPU micro architecture for optimizing memory system performance."

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac #convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- GPU
- Load
- Cache
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

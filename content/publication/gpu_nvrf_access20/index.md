---
title: "Hi-End: Hierarchical, Endurance-Aware STT-MRAM-Based Register File for Energy-Efficient GPUs"
authors:
- Won Jeon
- Jun Hyun Park
- Yoonsoo Kim
- admin
- Won Woo Ro
author_notes:
- "Equal contribution"
- "Equal contribution"
date: "2020-07-13T00:00:00Z"
doi: "10.1109/ACCESS.2020.3008719"

# Schedule page publish date (NOT publication's date).
publishDate: "2020-07-13T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Access* (Volume: 8)"
publication_short: "*IEEE Access*"

abstract: Modern Graphics Processing Units (GPUs) require large hardware resources for massive parallel thread executions. In particular, modern GPUs have a large register file composed of Static Random Access Memory (SRAM). Due to the high leakage current of SRAM, the register file consumes approximately 20% of the total GPU energy. The energy efficiency of the register file becomes more critical as the throughput of GPUs increases. For more energy-efficient GPUs, the usage of non-volatile memory such as Spin-Transfer Torque Magnetic Random Access Memory (STT-MRAM) as the GPU register file has been studied extensively. STT-MRAM requires a lower leakage current compared to SRAM and provides an appropriate read performance. However, using STT-MRAM directly in the GPU register file causes problems in performance and endurance because of complicated write procedures and material characteristics. To overcome these challenges, we propose a novel register file architecture and its management system for GPUs, named Hi-End, which exploits the data locality and compressibility of the register file. For STT-MRAM-based GPU register files, Hi-End increases the data write performance and endurance by caching and data compression, respectively. In our evaluation, Hi-End enhances the energy efficiency of a GPU register file by 70.02% and reduces the write operations by up to 95.98% with negligible performance degradation compared to SRAM-based register files.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- GPU
- Register File
- STT-MRAM
- Energy Efficiency
- Data Compression
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: http://arxiv.org/pdf/1512.04133v1
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
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: ""
  preview_only: false

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
slides:
---

#{{% callout note %}}
#Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
#{{% /callout %}}
#
#Supplementary notes can be added here, including [code and math](https://sourcethemes.com/academic/docs/writing-markdown-latex/).

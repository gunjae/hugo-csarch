---
title: "Improving Energy Efficiency of GPUs through Data Compression and Compressed Execution"
authors:
- Sangpil Lee
- Keunsoo Kim
- admin
- Hyeran Jeon
- Won Woo Ro
- Murali Annavaram
date: "2017-05-01T00:00:00Z"
doi: "10.1109/TC.2016.2619348"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-05-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Computers* (Volume: 66, Issue 5)"
publication_short: "*TC*"

abstract: "GPU design trends show that the register file size will continue to increase to enable even more thread level parallelism. As a result register file consumes a large fraction of the total GPU chip power. This paper explores register file data compression for GPUs to improve power efficiency. Compression reduces the width of the register file read and write operations, which in turn reduces dynamic power. This work is motivated by the observation that the register values of threads within the same warp are similar, namely the arithmetic differences between two successive thread registers is small. Compression exploits the value similarity by removing data redundancy of register values. Without decompressing operand values some instructions can be processed inside register file, which enables to further save energy by minimizing data movement and processing in power hungry main execution unit. Evaluation results show that the proposed techniques save 25 percent of the total register file energy consumption and 21 percent of the total execution unit energy consumption with negligible performance impact."

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- GPU
- Register File
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

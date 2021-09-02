---
title: "Warped-Compression: Enabling Power Efficient GPUs through Register Compression"
authors:
- Sangpil Lee
- Keunsoo Kim
- admin
- Hyeran Jeon
- Won Woo Ro
- Murali Annavaram
date: "2015-06-13T00:00:00Z"
doi: "10.1145/2749469.2750417"

# Schedule page publish date (NOT publication's date).
publishDate: "2015-06-13T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*International Symposium on Computer Architecture*"
publication_short: "*ISCA '15*"

abstract: "This paper presents Warped-Compression, a warp-level register compression scheme for reducing GPU power consumption. This work is motivated by the observation that the register values of threads within the same warp are similar, namely the arithmetic differences between two successive thread registers is small. Removing data redundancy of register values through register compression reduces the effective register width, thereby enabling power reduction opportunities. GPU register files are huge as they are necessary to keep concurrent execution contexts and to enable fast context switching. As a result register file consumes a large fraction of the total GPU chip power. GPU design trends show that the register file size will continue to increase to enable even more thread level parallelism. To reduce register file data redundancy warped-compression uses low-cost and implementation-efficient base-delta-immediate (BDI) compression scheme, that takes advantage of banked register file organization used in GPUs. Since threads within a warp write values with strong similarity, BDI can quickly compress and decompress by selecting either a single register, or one of the register banks, as the primary base and then computing delta values of all the other registers, or banks. Warped-compression can be used to reduce both dynamic and leakage power. By compressing register values, each warp-level register access activates fewer register banks, which leads to reduction in dynamic power. When fewer banks are used to store the register content, leakage power can be reduced by power gating the unused banks. Evaluation results show that register compression saves 25% of the total register file power consumption."

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac #convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- GPU
- Register File
- Data Compression
- Energy Efficiency
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

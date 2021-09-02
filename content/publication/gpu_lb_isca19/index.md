---
title: "Linebacker: Preserving Victim Cache Lines in Idle Register Files of GPUs"
authors:
- Yunho Oh
- admin
- Murali Annavaram
- Won Woo Ro
date: "2019-06-26T00:00:00Z"
doi: "10.1145/3307650.3322222"

# Schedule page publish date (NOT publication's date).
publishDate: "2019-06-26T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*International Symposium on Computer Architecture*"
publication_short: "*ISCA '19*"

abstract: "Modern GPUs suffer from cache contention due to the limited cache size that is shared across tens of concurrently running warps. To increase the per-warp cache size prior techniques proposed warp throttling which limits the number of active warps. Warp throttling leaves several registers to be dynamically unused whenever a warp is throttled. Given the stringent cache size limitation in GPUs this work proposes a new cache management technique named Linebacker (LB) that improves GPU performance by utilizing idle register file space as victim cache space. Whenever a CTA becomes inactive, linebacker backs up the registers of the throttled CTA to the off-chip memory. Then, linebacker utilizes the corresponding register file space as victim cache space. If any load instruction finds data in the victim cache line, the data is directly copied to the destination register through a simple register-register move operation. To further improve the efficiency of victim cache linebacker allocates victim cache space only to a select few load instructions that exhibit high data locality. Through a careful design of victim cache indexing and management scheme linebacker provides 29.0% of speedup compared to the previously proposed warp throttling techniques."

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac #convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- GPU
- Cache
- Register File
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

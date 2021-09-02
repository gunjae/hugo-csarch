---
title: "GraphSSD: Graph Semantics Aware SSD"
authors:
- Kiran Kumar Matam
- admin
- Haipeng Zha
- Hung-Wei Tseng
- Murali Annavaram
date: "2019-06-26T00:00:00Z"
doi: "10.1145/3307650.3322275"

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

abstract: "Graph analytics play a key role in a number of applications such as social networks, drug discovery, and recommendation systems. Given the large size of graphs that may exceed the capacity of the main memory, application performance is bounded by storage access time. Out-of-core graph processing frameworks try to tackle this storage access bottleneck through techniques such as graph sharding, and sub-graph partitioning. Even with these techniques, the need to access data across different graph shards or sub-graphs causes storage systems to become a significant performance hurdle. In this paper, we propose a graph semantic aware solid state drive (SSD) framework, called GraphSSD, which is a full system solution for storing, accessing, and performing graph analytics on SSDs. Rather than treating storage as a collection of blocks, GraphSSD considers graph structure while deciding on graph layout, access, and update mechanisms. GraphSSD replaces the conventional logical to physical page mapping mechanism in an SSD with a novel vertex-to-page mapping scheme and exploits the detailed knowledge of the flash properties to minimize page accesses. GraphSSD also supports efficient graph updates (vertex and edge modifications) by minimizing unnecessary page movement overheads. GraphSSD provides a simple programming interface that enables application developers to access graphs as native data in their applications, thereby simplifying the code development. It also augments the NVMe (non-volatile memory express) interface with a minimal set of changes to map the graph access APIs to appropriate storage access mechanisms. 
Our evaluation results show that the GraphSSD framework improves the performance by up to 1.85 × for the basic graph data fetch functions and on average 1.40×, 1.42×, 1.60×, 1.56×, and 1.29× for the widely used breadth-first search, connected components, random-walk, maximal independent set, and page rank applications, respectively."

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac #convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- SSD
- Storage
- Graphs
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

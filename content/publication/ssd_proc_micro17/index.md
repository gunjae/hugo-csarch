---
title: "Summarizer: Trading Communication with Computing near Storage"
authors:
- admin
- Kiran Kumar Matam
- Te I
- H. V. Krishna Giri Narra
- Jing Li
- Hung-Wei Tseng
- Steven Swanson
- Murali Annavaram
author_notes:
- "Equal contribution"
- "Equal contribution"
date: "2017-10-14T00:00:00Z"
doi: "10.1145/3123939.3124553"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-10-14T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*International Symposium on Microarchitecture*"
publication_short: "*MICRO '17*"

abstract: "Modern data center solid state drives (SSDs) integrate multiple general-purpose embedded cores to manage flash translation layer, garbage collection, wear-leveling, and etc., to improve the performance and the reliability of SSDs. As the performance of these cores steadily improves there are opportunities to repurpose these cores to perform application driven computations on stored data, with the aim of reducing the communication between the host processor and the SSD. Reducing host-SSD bandwidth demand cuts down the I/O time which is a bottleneck for many applications operating on large data sets. However, the embedded core performance is still significantly lower than the host processor, as generally wimpy embedded cores are used within SSD for cost effective reasons. So there is a trade-off between the computation overhead associated with near SSD processing and the reduction in communication overhead to the host system.
In this work, we design a set of application programming interfaces (APIs) that can be used by the host application to offload a data intensive task to the SSD processor. We describe how these APIs can be implemented by simple modifications to the existing Non-Volatile Memory Express (NVMe) command interface between the host and the SSD processor. We then quantify the computation versus communication tradeoffs for near storage computing using applications from two important domains, namely data analytics and data integration. Using a fully functional SSD evaluation platform we perform design space exploration of our proposed approach by varying the bandwidth and computation capabilities of the SSD processor. We evaluate static and dynamic approaches for dividing the work between the host and SSD processor, and show that our design may improve the performance by up to 20% when compared to processing at the host processor only, and 6X when compared to processing at the SSD processor only."

# Summary. An optional shortened abstract.
#summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac #convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- SSD
- Near Data Processing
- Dynamic Workload Offloading
- Storage Systems
featured: true

links:
- name: Slide Show
  url: https://filedn.com/luEeJVCCazShDlU4ibloXvu/publication/ssd_proc_micro17/ssd_proc_micro17_slides.ppsx
url_pdf: https://filedn.com/luEeJVCCazShDlU4ibloXvu/publication/ssd_proc_micro17/ssd_proc_micro17.pdf
url_code: ''
url_dataset: ''
url_poster: https://filedn.com/luEeJVCCazShDlU4ibloXvu/publication/ssd_proc_micro17/ssd_proc_micro17_poster.pdf
url_project: ''
url_slides: https://filedn.com/luEeJVCCazShDlU4ibloXvu/publication/ssd_proc_micro17/ssd_proc_micro17_slides.pdf
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  caption: 'Summarizer firmware architecture'
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

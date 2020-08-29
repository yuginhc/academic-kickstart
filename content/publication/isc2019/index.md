---
title: "Distributed Deep Learning with FPGA Ring Allreduce"
authors:
- Kenji Tanaka
- Yuki Arikawa
- Kenji Kawai
- Junichi Kato
- Tsuyoshi Ito
- Huy Cu Ngo
- Kazutaka Morita
- Fumiaki Miura
- Takeshi Sakamoto
- Satoshi Shigematsu

date: "2019-06-18T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2019-06-18T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *International Supercomputing Conference*
publication_short: In *ISC*

abstract: Among various methods for efficient distributed Deep Learning (DL), the top three state-of-the-art ImageNet/ResNet-50 training were achieved by utilizing a distributed data-parallel DL with Ring Allreduce or 2D-Torus Allreduce. However, it is difficult to apply them at large scale because latency is accumulated at each node due to data moving to GPU or CPU for Reduce processes. Our solution is to use In-Network Computing to handle data reduction while it is being transferred in the network. Since the conventional In-Network Computing system can apply to only hierarchical Allreduce, in this work, we propose a new In-Network Computing system that can support Ring Allreduce. In order to minimize communication overhead, we apply layer-based computing/communication overlap and optimize it for our proposed In-Network Computing system. We also propose a highly productive software stack consisting of a DL framework and heterogeneous device control languages. The evaluation results show that we can reduce the communication overhead by 84.27% at a batch size of 32 without any accuracy degradation. Moreover, the total learning time can be reduced by 7% when using 4 nodes learning system. It is confirmed that our system can significantly reduce the communication overhead without deteriorating accuracy when applying to a large-scale distributed DL with a large communication load. Although the current top data is 2-D Torus Allreduce using ASIC in domain specific architecture, the result shows that the communication overhead is shorter by applying the proposed system, which indicates the possibility of In-Network Computing.

# Summary. An optional shortened abstract.
summary: In this work, we propose a new In-Network Computing system that can support Ring Allreduce. In order to minimize communication overhead, we apply layer-based computing/communication overlap and optimize it for our proposed In-Network Computing system.

tags:
- isc
- distributed deep learning
- FPGA accelerator
- In-Network Computing
featured: true

links:
- name: Link
  url: https://2019.isc-program.com/presentation/?id=post120&sess=sess182
url_pdf: https://ssl.linklings.net/conferences/isc_hpc/assets/2019/posters/post120.pdf
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
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

<!-- 
{{% alert note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /alert %}}

{{% alert note %}}
Click the *Slides* button above to demo Academic's Markdown slides feature.
{{% /alert %}}

Supplementary notes can be added here, including [code and math](https://sourcethemes.com/academic/docs/writing-markdown-latex/). -->


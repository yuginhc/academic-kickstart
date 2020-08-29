---
title: "Large-Message Size Allreduce at Wire Speed for Distributed Deep Learning"
authors:
- Kenji Tanaka
- Yuki Arikawa
- Kenji Kawai
- Junichi Kato
- Tsuyoshi Ito
- Huy Cu Ngo
- Kazutaka Morita
- Takeshi Sakamoto
- Satoshi Shigematsu

date: "2018-11-18T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2018-11-18T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *The International Conference for High Performance Computing, Networking, Storage, and Analysis*
publication_short: In *SC*

abstract:  In large-scale distributed deep learning, the Allreduce operation for large messages (100 KB or more) is critical for gathering gradients from multiple worker nodes and broadcasting the sum of the gradients to them. When the message is large, the latency in Allreduce operation would make it difficult to take advantage of large-scale distributed deep learning. To reduce the latency, we devised a dataflow architecture with an Allreduce-specific hardware accelerator that performs data aggregation and reduction while data is being transferred. The accelerator is designed to immediately start Allreduce operation before an entire message is recived. Furthermore, Allreduce can be operated at wire speed by vectorizing the gradients and summing them in parallel. Experimental results reveal that the proposed architecture performs Allreduce at 96% of wire speed for a large message. Moreover, the latency of Allreduce is reduced by 65% compared with a state-of-the-art Allreduce method when applied for ResNet-50.

# Summary. An optional shortened abstract.
summary: To reduce the latency, we devised a dataflow architecture with an Allreduce-specific hardware accelerator that performs data aggregation and reduction while data is being transferred. The accelerator is designed to immediately start Allreduce operation before an entire message is recived.

tags:
- sc
- distributed deep learning
- FPGA accelerator
- In-Network Computing
featured: true

links:
- name: Link
  url: https://sc18.supercomputing.org/proceedings/tech_poster/tech_poster_pages/post140.html
url_pdf: https://sc18.supercomputing.org/proceedings/tech_poster/poster_files/post140s2-file2.pdf
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


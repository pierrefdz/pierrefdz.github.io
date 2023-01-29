---
layout: publication_page
show: true
noheader: true

title: Active Image Indexing
description: 

date: 2022-10-15

authors:
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [Facebook AI Research, INRIA]
  - name: Matthijs Douze
    url: "https://scholar.google.com/citations?user=0eFZtREAAAAJ&hl=en"
    affiliations: [Facebook AI Research]
  - name: Hervé Jégou
    url: "https://scholar.google.com/citations?user=1lcY2z4AAAAJ&hl=en"
    affiliations: [Facebook AI Research]
  - name: Teddy Furon
    url: "https://scholar.google.com/citations?hl=en&user=aLUbWzAAAAAJ"
    affiliations: [INRIA]

bib: /assets/bibliography/activeindexing.txt
pdf: /assets/publis/activeindexing/paper.pdf 
arxiv: https://arxiv.org/abs/2210.10620
publisher: https://openreview.net/forum?id=K9RHxPpjn2
img: /assets/publis/activeindexing/splash.png
code: https://github.com/facebookresearch/active_indexing

header-includes:
  - \usepackage[ruled,vlined,linesnumbered]{algorithm2e}
---

## TL;DR (Summary)

### Context

Image copy detection and retrieval from large databases leverage two components. First, a neural network maps an image to a vector representation, that is relatively robust to various transformations of the image. Second, an efficient but approximate similarity search algorithm trades scalability (size and speed) against quality of the search, thereby introducing a source of error. 

### The idea behind Active Indexing

We improve the robustness of copy detection on an image by modifying it in an imperceptible manner before its release (like in watermarking). The goal is to push the image's representation deep into its indexing partition.

*How?* We back-propagate a loss from the deep neural network back to the image, under perceptual constraints. 
Our experiments show that the retrieval and copy detection of activated images is significantly improved. For instance, activation improves by $+40$% the Recall1@1 on various image transformations, and for several popular indexing structures based on product quantization or locality sensitivity hashing.

*When?*  The method could apply whenever Alice distributes images and wants to moderate versions edited and shared by Bobs over the web. For example, stock photography providers (like Shutterstock, Getty) or Digital Asset Management companies that want to check that their pictures are rightfully credited. They would just distribute images activated for the index and feature extractor they use for indexing. Another example can be with generative image models (DALL.E and Stable Diffusion) and APIs distributed by OpenAI and HuggingFace. 
Compared to watermarking, the method leverage the access to the original images, which makes it better than watermarking for the task of copy detection.

## Poster


## Links

- [`arXiv`]({{page.arxiv}})
- [`OpenReview`]({{page.publisher}})
- [`PDF`]({{page.pdf}})

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
    affiliations: [FAIR Meta, Inria]
  - name: Matthijs Douze
    url: "https://scholar.google.com/citations?user=0eFZtREAAAAJ&hl=en"
    affiliations: [FAIR Meta]
  - name: Hervé Jégou
    url: "https://scholar.google.com/citations?user=1lcY2z4AAAAJ&hl=en"
    affiliations: [FAIR Meta]
  - name: Teddy Furon
    url: "https://scholar.google.com/citations?hl=en&user=aLUbWzAAAAAJ"
    affiliations: [Inria]

journal: International Conference on Learning Representations (ICLR)
bib: /assets/bibliography/activeindexing.txt
pdf: /assets/publis/activeindexing/paper.pdf 
arxiv: https://arxiv.org/abs/2210.10620
publisher: https://openreview.net/forum?id=K9RHxPpjn2
img: /assets/publis/activeindexing/splash.png
code: https://github.com/facebookresearch/active_indexing

header-includes:
  - \usepackage[ruled,vlined,linesnumbered]{algorithm2e}
---

## Abstract

*Context* 
- Image copy detection and retrieval from large databases leverage two components. 
First, a neural network maps an image to a vector representation, that is relatively robust to various transformations of the image. Second, an efficient but approximate similarity search algorithm trades scalability (size and speed) against quality of the search, thereby introducing a source of error. 
- We improve the robustness of copy detection on an image by modifying it in an imperceptible manner before its release (like in watermarking). The goal is to push the image's representation deep into its indexing partition.

<img src="/assets/publis/activeindexing/animated.gif" class="img-fluid thumbnail mt-2" alt="Active Indexing - overview">
  

*How?*
- We back-propagate a loss from the deep neural network back to the image, under perceptual constraints. 
- Our experiments show that the retrieval and copy detection of activated images is significantly improved. For instance, activation improves by +40% the Recall1@1 on various image transformations, and for several popular indexing structures based on product quantization or locality sensitivity hashing.

*When?*
- The method could apply whenever Alice distributes images and wants to moderate versions edited and shared by Bobs over the web. For example, stock photo banks (like Shutterstock, Getty, DALL·E, etc.) that want to check that their pictures are rightfully credited. 
They would just distribute images activated for the index and feature extractor they use for indexing.
- Compared to watermarking, the method leverages the access to the original images, which makes it better than blind watermarking for the task of copy detection.

## Poster

<img src="/assets/publis/activeindexing/poster.png" class="img-fluid thumbnail mt-2"> 

## Slides

<p align="center" class="img-fluid mt-2">
  <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vTJk9dylhB4Pmwbt-lYPH3YWHsEfW3VMMGdW7bKwr55ukdb-IiXsQRkjAlRQX1CCXnVJwqIIP1l562x/embed?start=false&loop=false&delayms=1000" frameborder="0" class="video" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
</p>

<!-- ## Video

<p align="center"><iframe width="560" height="315" src="" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p> -->

## Links

- [`arXiv`]({{page.arxiv}})
- [`OpenReview`]({{page.publisher}})
- [`Code`]({{page.code}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})
- [`Slides`](https://docs.google.com/presentation/d/122l94QY3Vj6UF8hKm83jBUU2aIk82Dh9AyAHqIZrRpY/)
- [`Video`](https://recorder-v3.slideslive.com/?share=79208&s=1dcd4f29-eb77-4fb7-85ec-843dab4215b6)


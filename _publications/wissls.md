---
layout: publication_page
show: true
noheader: true

title: Watermarking Images in Self-Supervised Latent Spaces
description: 

date: 2021-12-27

authors:
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [Facebook AI Research, INRIA]
  - name: Alexandre Sablayrolles
    url: "https://alexandresablayrolles.github.io/"
    affiliations: [Facebook AI Research]
  - name: Teddy Furon
    url: "https://scholar.google.com/citations?hl=en&user=aLUbWzAAAAAJ"
    affiliations: [INRIA]
  - name: Hervé Jégou
    url: "https://scholar.google.com/citations?user=1lcY2z4AAAAJ&hl=en"
    affiliations: [Facebook AI Research]
  - name: Matthijs Douze
    url: "https://scholar.google.com/citations?user=0eFZtREAAAAJ&hl=en"
    affiliations: [Facebook AI Research]

journal: ArXiv
bib: /assets/bibliography/wissls.txt
abstract: We revisit watermarking techniques based on pre-trained deep networks, in the light of self-supervised approaches. We present a way to embed both marks and binary messages into their latent spaces, leveraging data augmentation at marking time. Our method can operate at any resolution and creates watermarks robust to a broad range of transformations (rotations, crops, JPEG, contrast, etc). It significantly outperforms the previous zero-bit methods, and its performance on multi-bit watermarking is on par with state-of-the-art encoder-decoder architectures trained end-to-end for watermarking. Our implementation and models will be made publicly available.
pdf: /assets/pdf/wissls.pdf 
arxiv: https://arxiv.org/abs/2112.09581
img: /assets/img/wissls/splash.png

# Below is an example of injecting additional page-specific styles.
# If you use this page as a template, delete this _styles block.
_styles: >
  # .fake-img {
  #   background: #bbb;
  #   border: 1px solid rgba(0, 0, 0, 0.1);
  #   box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
  #   margin-bottom: 12px;
  # }
  # .fake-img p {
  #   font-family: monospace;
  #   color: white;
  #   text-align: left;
  #   margin: 12px 0;
  #   text-align: center;
  #   font-size: 16px;
  # }
---

## Downloads

- [PDF]({{page.pdf}})
- [Intership Report](/assets/pdf/wissls_internship.pdf)
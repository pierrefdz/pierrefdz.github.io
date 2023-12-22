---
layout: publication_page
show: true
noheader: true

title: 'Functional Invariants to Watermark Large Transformers'
description: 

date: 2023-10-17

authors:
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta, Inria]
  - name: Guillaume Couairon
    url: "https://scholar.google.com/citations?user=O1DeDyEAAAAJ&hl=en"
    affiliations: [FAIR Meta]
  - name: Teddy Furon
    url: "https://scholar.google.com/citations?hl=en&user=aLUbWzAAAAAJ"
    affiliations: [Inria]
  - name: Matthijs Douze
    url: "https://scholar.google.com/citations?user=0eFZtREAAAAJ&hl=en"
    affiliations: [FAIR Meta]

journal: International Conference on Acoustics, Speech, and Signal Processing (ICASSP)
arxiv: https://arxiv.org/abs/2310.11446
bib: /assets/bibliography/invariancewm.txt
pdf: /assets/publis/invariancewm/paper.pdf 
img: /assets/publis/invariancewm/splash.png

---

## TL;DR (Summary)

A training-free watermark for transformers that leverages the models' invariance through operations like dimension permutations or scaling/unscaling. The goal is to embed an identifier into the model weights to trace leaks.

## Abstract

The rapid growth of transformer-based models increases the concerns about their integrity and ownership insurance. Watermarking addresses this issue by embedding a unique identifier into the model, while preserving its performance. However, most existing approaches require to optimize the weights to imprint the watermark signal, which is not suitable at scale due to the computational cost. This paper explores watermarks with virtually no computational cost, applicable to a non-blind white-box setting (assuming access to both the original and watermarked networks). They generate functionally equivalent copies by leveraging the models' invariance, via operations like dimension permutations or scaling/unscaling. This enables to watermark models without any change in their outputs and remains stealthy. Experiments demonstrate the effectiveness of the approach and its robustness against various model transformations (fine-tuning, quantization, pruning), making it a practical solution to protect the integrity of large models.

## Links

- [`PDF`]({{page.pdf}})
- [`arXiv`]({{page.arxiv}})
- [`BibTeX`]({{page.bib}})

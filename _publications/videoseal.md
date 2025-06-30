---
layout: publication_page
show: true
noheader: true

title: "Video Seal: Open and Efficient Video Watermarking"
description: Official implementation of Video Seal: Open and Efficient Video Watermarking

date: 2024-12-17

authors:
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]
  - name: Hady Elsahar
  - name: I. Zeki Yalniz
  - name: Alexandre Mourachko

journal: arXiv preprint arXiv:2412.09492
bib: /assets/bibliography/videoseal.txt
pdf: https://arxiv.org/pdf/2412.09492.pdf
arxiv: https://arxiv.org/abs/2412.09492
code: https://github.com/facebookresearch/videoseal
img: /assets/publis/videoseal/splash.png

header-includes:
  - \usepackage[ruled,vlined,linesnumbered]{algorithm2e}
---

<!-- center -->
<p align="center">
  <img src="{{ page.img }}" class="img-fluid thumbnail mt-2" style="max-width: 75%;">
</p>

Video Seal introduces a novel open-source framework for neural video watermarking, combining a jointly trained embedder and extractor to ensure robustness and efficiency. The method leverages multistage training—image pre-training, hybrid post-training, and extractor fine-tuning—alongside temporal watermark propagation to avoid per-frame embedding. Differentiable augmentations, including common video codecs, are applied during training to simulate real-world transformations and improve resilience.

The accompanying codebase provides end-to-end pipelines for training and inference. Key assets include TorchScript models, training scripts (`train.py`), inference tools (`inference_av.py`, `inference_streaming.py`), evaluation modules (`videoseal/evals/full.py`), and Jupyter notebooks for interactive exploration. Pre-trained checkpoints and a live demo endpoint are also available to facilitate rapid experimentation.

## Quick Start

Official implementation of Video Seal: Open and Efficient Video Watermarking. State-of-the-art open-sourced models for video and image watermarking.

## Links

- [`Paper`](https://ai.meta.com/research/publications/video-seal-open-and-efficient-video-watermarking/)
- [`arXiv`]({{ page.arxiv }})
- [`Code`]({{ page.code }})
- [`PDF`]({{ page.pdf }})
- [`BibTeX`]({{ page.bib }})
- [`Demo`](https://aidemos.meta.com/videoseal)

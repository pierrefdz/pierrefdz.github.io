---
layout: publication_page
show: true
noheader: true

title: 'Video Seal: Open and Efficient Video Watermarking'
description: 

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

---

<img src="/assets/publis/videoseal/splash.png" 
class="img-fluid thumbnail mt-2" alt="Active Indexing - overview">

Video Seal introduces a novel open-source framework for neural video watermarking, combining a jointly trained embedder and extractor to ensure robustness and efficiency. The method leverages multistage training—image pre-training, hybrid post-training, and extractor fine-tuning—alongside temporal watermark propagation to avoid per-frame embedding. Differentiable augmentations, including common video codecs, are applied during training to simulate real-world transformations and improve resilience.

The accompanying codebase provides end-to-end pipelines for training and inference. Key assets include TorchScript models, training scripts (`train.py`), inference tools (`inference_av.py`, `inference_streaming.py`), evaluation modules (`videoseal/evals/full.py`), and Jupyter notebooks for interactive exploration. Pre-trained checkpoints and a live demo endpoint are also available to facilitate rapid experimentation.


## Links

- [`Paper`](https://ai.meta.com/research/publications/video-seal-open-and-efficient-video-watermarking/)
- [`arXiv`]({{ page.arxiv }})
- [`Code`]({{ page.code }})
- [`PDF`]({{ page.pdf }})
- [`BibTeX`]({{ page.bib }})
- [`Demo`](https://aidemos.meta.com/videoseal)

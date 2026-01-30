---
layout: publication_page
show: true
noheader: true

title: 'Pixel Seal: Adversarial-only Training for Invisible Image and Video Watermarking'
description: 

date: 2025-12-18

authors:
  - name: Tomáš Souček
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]
  - name: Hady Elsahar
  - name: Sylvestre-Alvise Rebuffi
  - name: Valeriu Lacatusu
  - name: Tuan Tran
  - name: Tom Sander
  - name: Alexandre Mourachko

journal: arXiv preprint arXiv:2512.16874
bib: /assets/publis/pixelseal/bib.txt
pdf: /assets/publis/pixelseal/paper.pdf
arxiv: https://arxiv.org/abs/2512.16874
img: /assets/publis/pixelseal/splash.png

---

<img src="/assets/publis/pixelseal/splash.png" 
class="img-fluid thumbnail mt-2" alt="Pixel Seal - overview">

Invisible watermarking is essential for tracing the provenance of digital content. However, training state-of-the-art models remains notoriously difficult, with current approaches often struggling to balance robustness against true imperceptibility. This work introduces Pixel Seal, which sets a new state-of-the-art for image and video watermarking.

We first identify three fundamental issues of existing methods: (i) the reliance on proxy perceptual losses such as MSE and LPIPS that fail to mimic human perception and result in visible watermark artifacts; (ii) the optimization instability caused by conflicting objectives, which necessitates exhaustive hyperparameter tuning; and (iii) reduced robustness and imperceptibility of watermarks when scaling models to high-resolution images and videos.

To overcome these issues, we first propose an adversarial-only training paradigm that eliminates unreliable pixel-wise imperceptibility losses. Second, we introduce a three-stage training schedule that stabilizes convergence by decoupling robustness and imperceptibility. Third, we address the resolution gap via high-resolution adaptation, employing JND-based attenuation and training-time inference simulation to eliminate upscaling artifacts.

## Links

- [`arXiv`]({{ page.arxiv }})
- [`PDF`]({{ page.pdf }})
- [`BibTeX`]({{ page.bib }})

---
layout: publication_page
show: true
noheader: true

title: 'Geometric Image Synchronization with Deep Watermarking'
description: 

date: 2025-09-18

authors:
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]
  - name: Tomáš Souček
  - name: Nikola Jovanović
    url: "https://scholar.google.com/citations?user=nE1czKQAAAAJ&hl=en"
  - name: Hady Elsahar
  - name: Sylvestre-Alvise Rebuffi
  - name: Valeriu Lacatusu
  - name: Tuan Tran
  - name: Alexandre Mourachko

journal: arXiv preprint arXiv:2509.15208
bib: /assets/bibliography/syncseal.txt
pdf: https://arxiv.org/pdf/2509.15208.pdf
arxiv: https://arxiv.org/abs/2509.15208
code: https://github.com/facebookresearch/wmar/tree/main/syncseal
img: /assets/publis/syncseal/splash.png

---

<img src="/assets/publis/syncseal/splash.png" 
class="img-fluid thumbnail mt-2" alt="SyncSeal - overview">

Synchronization is the task of estimating and inverting geometric transformations (e.g., crop, rotation) applied to an image. This work introduces SyncSeal, a bespoke watermarking method for robust image synchronization, which can be applied on top of existing watermarking methods to enhance their robustness against geometric transformations. It relies on an embedder network that imperceptibly alters images and an extractor network that predicts the geometric transformation to which the image was subjected. Both networks are end-to-end trained to minimize the error between the predicted and ground-truth parameters of the transformation, combined with a discriminator to maintain high perceptual quality. We experimentally validate our method on a wide variety of geometric and valuemetric transformations, demonstrating its effectiveness in accurately synchronizing images. We further show that our synchronization can effectively upgrade existing watermarking methods to withstand geometric transformations to which they were previously vulnerable.

## Links

- [`arXiv`](https://arxiv.org/abs/2509.15208)
- [`Code`](https://github.com/facebookresearch/wmar/tree/main/syncseal)
- [`PDF`](https://arxiv.org/pdf/2509.15208.pdf)
- [`BibTeX`]({{ page.bib }})

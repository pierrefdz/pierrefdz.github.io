---
layout: publication_page
show: true
noheader: true

title: 'TextSeal: A Localized LLM Watermark for Provenance & Distillation Protection'
description: 

date: 2026-05-12

authors:
  - name: "Tom Sander*"
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta]
  - name: Hongyan Chang
  - name: Sylvestre-Alvise Rebuffi
  - name: Tomáš Souček
  - name: Tuan Tran
  - name: Valeriu Lacatusu
  - name: Alexandre Mourachko
  - name: Surya Parimi
  - name: Christophe Ropers
  - name: Rashel Moritz
  - name: Vanessa Stark
  - name: Hady Elsahar
  - name: "Pierre Fernandez*"
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]

journal: Neural Information Processing Systems (NeurIPS)
bib: /assets/publis/textseal/bib.txt
pdf: /assets/publis/textseal/paper.pdf
arxiv: https://arxiv.org/abs/2605.12456
code: https://github.com/facebookresearch/textseal
img: /assets/publis/textseal/splash.png

---

<small>* Equal contribution.</small>

<img src="/assets/publis/textseal/splash.png" 
class="img-fluid thumbnail mt-2" alt="TextSeal - overview">

We introduce *TextSeal*, a state-of-the-art watermark for large language models. Building on Gumbel-max sampling, TextSeal introduces dual-key generation to restore output diversity, along with entropy-weighted scoring and multi-region localization for improved detection. It supports serving optimizations such as speculative decoding and multi-token prediction, and does not add any inference overhead.

TextSeal strictly dominates baselines like SynthID-text in detection strength and is robust to dilution, maintaining confident localized detection even in heavily mixed human/AI documents. The scheme is theoretically distortion-free, and evaluation across reasoning benchmarks confirms that it preserves downstream performance; while a multilingual human evaluation (6,000 A/B comparisons, 5 languages) shows no perceptible quality difference.

Beyond its use for provenance detection, TextSeal is also "radioactive": its watermark signal transfers through model distillation, enabling detection of unauthorized use.

## Links

- [`arXiv`]({{ page.arxiv }})
- [`Code`]({{ page.code }})
- [`PDF`]({{ page.pdf }})
- [`BibTeX`]({{ page.bib }})

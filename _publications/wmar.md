---
layout: publication_page
show: true
noheader: true

title: 'Watermarking Autoregressive Image Generation'
description: 

date: 2025-06-19

authors:
  - name: Nikola Jovanović
    url: "https://scholar.google.com/citations?user=nE1czKQAAAAJ&hl=en"
  - name: Ismail Labiad
  - name: Tomáš Souček
  - name: Martin Vechev
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]

journal: arXiv preprint arXiv:2506.16349
bib: /assets/bibliography/wmar.txt
pdf: https://arxiv.org/pdf/2506.16349.pdf
arxiv: https://arxiv.org/abs/2506.16349
code: https://github.com/facebookresearch/wmar
img: /assets/publis/wmar/splash.png

---

<img src="/assets/publis/wmar/splash.png" 
class="img-fluid thumbnail mt-2" alt="WMAR - overview">

Watermarking the outputs of generative models has emerged as a promising approach for tracking their provenance. Despite significant interest in autoregressive image generation models and their potential for misuse, no prior work has attempted to watermark their outputs at the token level. In this work, we present the first such approach by adapting language model watermarking techniques to this setting. We identify a key challenge: the lack of reverse cycle-consistency (RCC), wherein re-tokenizing generated image tokens significantly alters the token sequence, effectively erasing the watermark. To address this and to make our method robust to common image transformations, neural compression, and removal attacks, we introduce (i) a custom tokenizer-detokenizer finetuning procedure that improves RCC, and (ii) a complementary watermark synchronization layer. As our experiments demonstrate, our approach enables reliable and robust watermark detection with theoretically grounded p-values.

## Links

- [`arXiv`](https://arxiv.org/abs/2506.16349)
- [`Code`](https://github.com/facebookresearch/wmar)
- [`PDF`](https://arxiv.org/pdf/2506.16349.pdf)
- [`BibTeX`]({{ page.bib }})

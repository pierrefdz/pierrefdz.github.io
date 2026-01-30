---
layout: publication_page
show: true
noheader: true

title: 'How Good is Post-Hoc Watermarking With Language Model Rephrasing?'
description: 

date: 2025-12-18

authors:
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta]
  - name: Tom Sander
  - name: Hady Elsahar
  - name: Hongyan Chang
  - name: Tomáš Souček
  - name: Valeriu Lacatusu
  - name: Tuan Tran
  - name: Sylvestre-Alvise Rebuffi

journal: arXiv preprint arXiv:2512.16904
bib: /assets/publis/textseal/bib.txt
pdf: /assets/publis/textseal/paper.pdf
arxiv: https://arxiv.org/abs/2512.16904
img: /assets/publis/textseal/splash.png

---

<img src="/assets/publis/textseal/splash.png" 
class="img-fluid thumbnail mt-2" alt="Text Seal - overview">

Generation-time text watermarking embeds statistical signals into text for traceability of AI-generated content. We explore *post-hoc watermarking* where an LLM rewrites existing text while applying generation-time watermarking, to protect copyrighted documents, or detect their use in training or RAG via watermark radioactivity.

Unlike generation-time approaches, which is constrained by how LLMs are served, this setting offers additional degrees of freedom for both generation and detection. We investigate how allocating compute (through larger rephrasing models, beam search, multi-candidate generation, or entropy filtering at detection) affects the quality-detectability trade-off.

Our strategies achieve strong detectability and semantic fidelity on open-ended text such as books. Among our findings, the simple Gumbel-max scheme surprisingly outperforms more recent alternatives under nucleus sampling, and most methods benefit significantly from beam search. However, most approaches struggle when watermarking verifiable text such as code, where we counterintuitively find that smaller models outperform larger ones.

## Links

- [`arXiv`]({{ page.arxiv }})
- [`PDF`]({{ page.pdf }})
- [`BibTeX`]({{ page.bib }})

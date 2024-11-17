---
layout: publication_page
show: true
noheader: true

title: 'Watermarking Makes Language Models Radioactive'
description: 

date: 2024-02-26

authors:
  - name: Tom Sander
    url: "https://sandertom.github.io/"
    affiliations: [FAIR Meta, CMAP Ecole polytechnique]
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta, Inria]
  - name: Alain Durmus
    url: "https://alain.perso.math.cnrs.fr/"
    affiliations: [CMAP Ecole polytechnique]
  - name: Matthijs Douze
    url: "https://scholar.google.com/citations?user=0eFZtREAAAAJ&hl=en"
    affiliations: [FAIR Meta]
  - name: Teddy Furon
    url: "https://scholar.google.com/citations?hl=en&user=aLUbWzAAAAAJ"
    affiliations: [Inria]

journal: Neural Information Processing Systems (NeurIPS)
arxiv: https://arxiv.org/abs/2402.14904
bib: /assets/bibliography/radioactive.txt
pdf: /assets/publis/radioactive/paper.pdf 
img: /assets/publis/radioactive/splash.png


---

## TL;DR (Summary)

"Can people detect when you train on outputs from their LLM ?"
- Hard when outputs are not watermarked
- Easy when outputs are watermarked


## Abstract

This paper investigates the radioactivity of LLM-generated texts, i.e. whether it is possible to detect that such input was used as training data. Conventional methods like membership inference can carry out this detection with some level of accuracy. We show that watermarked training data leaves traces easier to detect and much more reliable than membership inference. We link the contamination level to the watermark robustness, its proportion in the training set, and the fine-tuning process. We notably demonstrate that training on watermarked synthetic instructions can be detected with high confidence (p-value < 1e-5) even when as little as 5% of training text is watermarked. Thus, LLM watermarking, originally designed for detecting machine-generated text, gives the ability to easily identify if the outputs of a watermarked LLM were used to fine-tune another LLM.

## Thread on Twitter

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">OpenAI may secretly know that you trained on GPT outputs!<br>In our work &quot;Watermarking Makes Language Models Radioactive&quot;, we show that training on watermarked text can be easily spotted ☢️ <br>Paper: <a href="https://t.co/EETij4oLF0">https://t.co/EETij4oLF0</a><a href="https://twitter.com/pierrefdz?ref_src=twsrc%5Etfw">@pierrefdz</a> <a href="https://twitter.com/AIatMeta?ref_src=twsrc%5Etfw">@AIatMeta</a> <a href="https://twitter.com/Polytechnique?ref_src=twsrc%5Etfw">@Polytechnique</a> <a href="https://twitter.com/Inria?ref_src=twsrc%5Etfw">@Inria</a> <a href="https://t.co/cjjyhp1DMg">pic.twitter.com/cjjyhp1DMg</a></p>&mdash; Tom Sander (@RednasTom) <a href="https://twitter.com/RednasTom/status/1762109247783891340?ref_src=twsrc%5Etfw">February 26, 2024</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

## Links

- [`arXiv`]({{page.arxiv}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})
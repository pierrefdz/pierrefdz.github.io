---
layout: publication_page
show: true
noheader: true

title: 'Seamless: Multilingual Expressive and Streaming Speech Translation'
description: 

date: 2023-11-30

authors:
  - name: Seamless Communication

journal: CoRR 2023
bib: /assets/bibliography/seamless.txt
pdf: /assets/publis/seamless/seamless.pdf 
arxiv: https://arxiv.org/abs/2312.05187
code: https://github.com/facebookresearch/seamless_communication
img: /assets/publis/seamless/splash.png

header-includes:
  - \usepackage[ruled,vlined,linesnumbered]{algorithm2e}
---

## Abstract

Recent advancements in automatic speech translation have dramatically expanded language coverage, improved multimodal capabilities, and enabled a wide range of tasks and functionalities. That said, large-scale automatic speech translation systems today lack key features that help machine-mediated communication feel seamless when compared to human-to-human dialogue. In this work, we introduce a family of models that enable end-to-end expressive and multilingual translations in a streaming fashion. First, we contribute an improved version of the massively multilingual and multimodal SeamlessM4T model—SeamlessM4T v2. This newer model, incorporating an updated UnitY2 framework, was trained on more low-resource language data. The expanded version of SeamlessAlign adds 114,800 hours of automatically aligned data for a total of 76 languages. SeamlessM4T v2 provides the foundation on which our two newest models, SeamlessExpressive and SeamlessStreaming, are initiated. SeamlessExpressive enables translation that preserves vocal styles and prosody. Compared to previous efforts in expressive speech research, our work addresses certain underexplored aspects of prosody, such as speech rate and pauses, while also preserving the style of one’s voice. As for SeamlessStreaming, our model leverages the Efficient Monotonic Multihead Attention (EMMA) mechanism to generate low-latency target translations without waiting for complete source utterances. As the first of its kind, SeamlessStreaming enables simultaneous speech-to-speech/text translation for multiple source and target languages. To understand the performance of these models, we combined novel and modified versions of existing automatic metrics to evaluate prosody, latency, and robustness. For human evaluations, we adapted existing protocols tailored for measuring the most relevant attributes in the preservation of meaning, naturalness, and expressivity. To ensure that our models can be used safely and responsibly, we implemented the first known red-teaming effort for multimodal machine translation, a system for the detection and mitigation of added toxicity, a systematic evaluation of gender bias, and an inaudible localized watermarking mechanism designed to dampen the impact of deepfakes. Consequently, we bring major components from SeamlessExpressive and SeamlessStreaming together to form Seamless, the first publicly available system that unlocks expressive cross-lingual communication in real-time. In sum, Seamless gives us a pivotal look at the technical foundation needed to turn the Universal Speech Translator from a science fiction concept into a real-world technology. Finally, contributions in this work—including models, code, and a watermark detector—are publicly released and accessible at the link below.

## Watermarking

Our team developed a watermarking method that proactively add an imperceptible watermark in the audio, which can be used to detect if a speech is AI-generated even in the presence of strong edit. It can pinpoint AI-generated segments in a longer audio with a sample level resolution (1/16k seconds).


## Links

<!-- - [`arXiv`]({{page.arxiv}}) -->
- [`Code`]({{page.code}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})
- [`Blog post`](https://ai.meta.com/research/seamless-communication/)
- [`Demo`](https://seamless.metademolab.com/expressive/?utm_source=metaai&utm_medium=web&utm_campaign=seamless&utm_content=landing_page)

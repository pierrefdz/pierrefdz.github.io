---
layout: publication_page
show: true
noheader: true

title: 'Proactive Detection of Voice Cloning with Localized Watermarking'
description: 

date: 2024-01-31

authors:
  - name: Robin San Roman
    url: "https://scholar.google.com/citations?user=AJ3ir84AAAAJ&hl=fr"
    affiliations: [FAIR Meta, Inria]
  - name: Pierre Fernandez
    url: "https://pierrefdz.github.io/"
    affiliations: [FAIR Meta, Inria]
  - name: Hady Elsahar
    url: "https://www.hadyelsahar.io/"
    affiliations: [FAIR Meta]
  - name: Teddy Furon
    url: "https://scholar.google.com/citations?hl=en&user=aLUbWzAAAAAJ"
    affiliations: [Inria]
  - name: Alexandre Défossez
    url: "https://ai.honu.io/"
    affiliations: [Kyutai]
  - name: Tuan Tran
    url: "https://scholar.google.de/citations?user=jk2BlO4AAAAJ&hl=en"
    affiliations: [FAIR Meta]

journal: arXiv (pre-print)
arxiv: https://arxiv.org/abs/2401.17264
bib: /assets/bibliography/audioseal.txt
pdf: /assets/publis/audioseal/paper.pdf 
img: /assets/publis/audioseal/splash.png
code: https://github.com/facebookresearch/audioseal


---

## TL;DR (Summary)

We introduce AudioSeal, a SOTA proactive solution for the detection of voice cloning or speech generation, based on a first-of-its-kind localized watermarking.

It beats passive detection methods by a huge margin. Compared to other watermarking methods, AudioSeal is perceptually better, has better robustness against edits and is ultra fast (can be used in real-time applications). And AudioSeal is pip installable!

## Towards better traceability of AI-generated speech with watermarking

The rise of AI-generated content poses challenges in ensuring authenticity and trustworthiness. 
Voice cloning, in particular, has the potential to deceive and manipulate individuals through the creation of synthetic voices that mimic real ones. 
Detection of these contents is at the same time crucial, to prevent their misuse and getting harder as the quality of the generated content improves.

To address this issue, we developed AudioSeal, a cutting-edge solution that leverages localized watermarking to detect AI-generated speech with precision.
Instead of relying on passive detection, AudioSeal proactively embeds a watermark into the speech signal, which can be later detected to verify the authenticity of the content.
The particularity of AudioSeal is that *the watermark detection is localized*. 
The detector directly predicts for each time step (1/16k of a second) if the watermark is present or not, which makes it ultra fast and suitable for real-time applications.

Previous iterations of AudioSeal were used to watermark generative models in public demos from 
AI at Meta, such as [Audiobox](https://audiobox.metademolab.com) and [Seamless](https://seamless.qa.metademolab.com/expressive), serving 100k users daily.



## How does it work?

<img src="/assets/publis/audioseal/overview.png" class="img-fluid thumbnail mt-2" alt="Overview. AudioSeal consists of a generator and a detector.">

AudioSeal consists of two main components:
- A generator, which generate an additive watermark waveform based on the input audio,
- A detector, which predicts the presence of the watermark at each time step.

The generator is trained to produce a watermark that is imperceptible to the human ear, and robust to common audio processing operations such as compression, re-encoding, and noise addition.
The detector is trained to predict the presence of the watermark at each time step, and is designed to be fast and suitable for real-life applications where watermarked audio is embedded in a stream of (often non-watermarked) audio.

### Model training


### Model architectures

### Detection, Localization and Attribution



## Main results

### Compared to passive detection

### Compared to the current SOTA watermarking method

### Watermark robustness to attacks


## Conclusion

AudioSeal represents a significant advancement for audio content detection, offering a proactive solution to combat the proliferation of AI-generated content. As technology continues to evolve, innovative approaches like AudioSeal play a crucial role in safeguarding the integrity of audio content and upholding responsibility in the deployments of these generative models.

## Links

- [`arXiv`]({{page.arxiv}})
- [`Code`]({{page.code}})
- [`PDF`]({{page.pdf}})
- [`BibTeX`]({{page.bib}})
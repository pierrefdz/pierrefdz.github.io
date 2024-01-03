---
layout: page
permalink: /
title: Home
description: PhD student at Inria and FAIR. Studied at École polytechnique and Paris-Saclay University.

profile:
  image: avatar.jpg
  address: >

nav: false
news: true  # includes a list of news items
---

## About me

<div class="row">
  <div class="col-md-8" markdown="1">
  Hi! 

  I am a PhD student at FAIR Paris (Fundamental AI Research lab at Meta) and INRIA Rennes, advised by [Matthijs Douze](https://scholar.google.fr/citations?user=0eFZtREAAAAJ&hl=fr), [Hervé Jégou](https://scholar.google.fr/citations?user=1lcY2z4AAAAJ&hl=fr) and [Teddy Furon](https://scholar.google.fr/citations?user=aLUbWzAAAAAJ&hl=fr). My research focuses on content protection and safety in machine learning, with a particular interest in generative models.

  Prior to my PhD, I studied at École polytechnique, majoring in computer science and mathematics for visual computing. I also hold a Master's degree from École des Ponts and from Paris-Saclay University.

  I am really excited in the developement of Artificial Intelligence and of its applications in the fields of every day's life. 
  </div>
  <div class="col-md-4 m-auto" style="text-align: center">
    <img class="img-responsive rounded-circle profile" src="assets/img/{{page.profile.image}}">
  </div>
</div>


## News

{% if page.news %}
  {% include news.html %}
{% endif %}

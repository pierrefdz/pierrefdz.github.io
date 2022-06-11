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
  Hi 🙋🏼‍♂️! 

  I am an AI Research PhD student at Meta AI & Inria Rennes, advised by [Matthijs Douze](https://scholar.google.fr/citations?user=0eFZtREAAAAJ&hl=fr), [Hervé Jégou](https://scholar.google.fr/citations?user=1lcY2z4AAAAJ&hl=fr) and [Teddy Furon](https://scholar.google.fr/citations?user=aLUbWzAAAAAJ&hl=fr). I am interested in data protection in the context of Machine Learning and Computer Vision.

  Prior to my PhD, I studied at École polytechnique, majoring in computer science and mathematics for visual computing. I also hold a Master's degree from École des Ponts and from Paris-Saclay University.

  I am really excited in the developement of Artificial Intelligence (more broadly Artificial Life) and of its applications in the fields of every day's life. 
  </div>
  <div class="col-md-4 m-auto" style="text-align: center">
    <img class="img-responsive rounded-circle profile" src="assets/img/{{page.profile.image}}">
  </div>
</div>


## News

{% if page.news %}
  {% include news.html %}
{% endif %}

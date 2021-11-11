---
layout: page
permalink: /
title: Home
description: Graduate student at École polytechnique and Paris-Saclay University, majoring in Mathematics & Computer Science

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

  I am a graduate student at Ecole polytechnique studying Machine Learning and Computer Vision. I am also pursuing a Master's degree in Mathematics, Vision and Learning at Paris-Saclay University in partnership with Ponts Paris-Tech. 

  I am really excited in the developement of Artificial Intelligence (more broadly Artificial Life) and of its applications in the fields of every day's life. I am interested in many topics related to computer vision, computer graphics and machine learning, particularly:
  - Fairness & privacy in computer vision applications
  - Soft robotics and evolutionary robotics

  At the moment, I work as an intern at Facebook AI Research center in Paris, under the supervision of Hervé Jégou and Matthijs Douze.
  </div>
  <div class="col-md-4 m-auto" style="text-align: center">
    <img class="img-responsive rounded-circle profile" src="assets/img/{{page.profile.image}}">
  </div>
</div>


## News

{% if page.news %}
  {% include news.html %}
{% endif %}
---
layout: page
permalink: /publications/
title: Publications
description: Publications and projects. You can also find most up-to-date entries for my latest publications on the Google Scholar page.
nav: true
---

<div class="publications">
{% if site.publications %}
  <div class="table-responsive">
    <table class="table table-sm table-borderless">
    {% assign publications = site.publications | reverse %}
    {% for publication in publications %}
      {% include publication.html %}
    {% endfor %}
    </table>
  </div>
{% else %}
  <p>No news so far...</p>
{% endif %}

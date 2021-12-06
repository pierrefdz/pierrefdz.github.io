---
layout: page
permalink: /publications/
title: Publications
description: Publications and projects. You can also find most up-to-date entries for my latest publications on the Google Scholar page.
nav: true
---

<div class="publications">
  <div class="table-responsive">
    <table class="table table-sm table-borderless">
    {% assign publications = site.publications | reverse %}
    {% for publi in publications %}
      {% if publi.show %}
        {% include publication.html %}
      {% endif %}
    {% endfor %}
    </table>
  </div>

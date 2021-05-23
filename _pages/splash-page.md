---
title: "bk"
layout: splash
permalink: /
date: 2021-05-23T11:48:41-04:00
header:

{% assign author = page.author | default: page.authors[0] | default: site.author %}
{% assign author = site.data.authors[author] | default: author %}

{% if author.avatar %}
    <div class="author__avatar">
      {% if author.avatar contains "://" %}
        {% assign author_src = author.avatar %}
      {% else %}
        {% assign author_src = author.avatar | relative_url %}
      {% endif %}
    </div>

  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/unsplash-image-1.jpg
#  caption: "Photo credit: [****](https://unsplash.com)"

excerpt: "[He](http://my.pronoun.is/he) is an experienced [shop educator](https://en.wikipedia.org/wiki/Technology_education) whose general work and many interests are loosely documented on this site."
---
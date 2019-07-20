---
layout: collection
title: "Places"
collection: places
permalink: /places/
author_profile: false
---

A collection of notes on `places` for travel.

{% assign category = site.collection | group_by: 'category' %}
{% for item in category %}
  <!-- This is the category name -->
  <h2>{{item.name}}</h2>
  <ul>
    <!-- filter the categories, selecting only the current category in the loop -->
    {% assign portfolio = site.portfolio | where: 'category', item.name %}
    {% for entry in portfolio %}
    <li class="item">
      <h4 class="post-title">{{ entry.title }}</h4>
    </li>
    {% endfor %}
  </ul>
{% endfor %}

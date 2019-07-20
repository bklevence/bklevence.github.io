---
layout: collection2
title: "Places"
collection: places
permalink: /places/
author_profile: false
---

A collection of notes on `places` for travels.

<h1>States {{ page.state }}</h1>

{% for places in site.places %}
{% if places.state == page.state %}
{{ section.output }}
{% endif %}
{% endfor %}

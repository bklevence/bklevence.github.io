---
layout: collection2
title: "Places"
collection: places
permalink: /places/
author_profile: false
---

A collection of notes on `places` for travels.

<h1>Chapter {{ page.state }}</h1>

{% for section in site.sections %}
{% if section.state == page.state %}
{{ section.output }}
{% endif %}
{% endfor %}

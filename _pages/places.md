---
layout: collection
title: "Places"
collection: places
permalink: /places/
author_profile: false
---

A collection of notes on `places` for travel.

{% assign groups = site.places | group_by: "category" | sort: "name" %}
{% for group in groups %}
    {{ group.name }}
    {% for item in group.items %}
        {{item.abbrev}}
    {%endfor%}
{%endfor%}

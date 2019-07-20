---
layout: collection2
title: "Places"
collection: places
permalink: /places/
author_profile: false
---

A collection of notes on `places` for travels.

<h1>States {{ page.state }}</h1>

{% assign groups = site.my_collection | group_by: "state" | sort: "name" %}
{% for group in groups %}
    {{ group.name }}
    {% for item in group.items %}
        {{item.title}}
    {%endfor%}
{%endfor%}

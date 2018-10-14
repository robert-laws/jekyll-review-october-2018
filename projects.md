---
layout: default
title: Projects Page
---
# {{page.title}}

{% for project in site.projects %}

* [{{project.title}}]({{site.baserul}}{{project.url}})

{% endfor %}
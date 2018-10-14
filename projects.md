---
layout: default
title: Projects Page
---
# {{page.title}}

{% for project in site.projects %}

{{ project.content | markdownify }}

[{{project.title}}]({{site.baserul}}{{project.url}})

{% endfor %}
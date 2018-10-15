---
layout: default
title: Projects Page
---
# {{page.title}}

{% for project in site.projects %}

<!-- {{ project.content | markdownify }} -->

{:.project-list}
* [{{project.title}}]({{site.baserul}}{{project.url}})
{% endfor %}

---

{:.project-list}
{% for project in site.data.projects %}
1. {{project.name}} - technology used: {{project.tech}}
{% endfor %}
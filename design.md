---
title: "Design Process"
process_order: 2
---
<!-- Design is an essential part of the process in creating a new website.

{{site.title}}

![Drink Coffee]({{site.baseurl}}/assets/img/photo78.jpg){:.medium-image}

This stage in the process requires a lot of focus.

--- -->

{% assign dog_daycare_process = site.dog_daycare | sort: 'process_order' %}

{% for process in dog_daycare_process %}

### {{process.title}}

{{process.content}}

---

{% endfor %}
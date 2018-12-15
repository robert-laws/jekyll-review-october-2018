---
layout: default
title: My Blog
---
# {{page.title}}

{% for post in site.posts %}

#### [{{post.title}}]({{site.baseurl}}{{post.url}})

{% endfor %}



<h1>{{page.title}}</h1>

<h2>I give this plugin two :smile: :+1:!</h2>

<h2>{% avatar robert-laws %}</h2>
<span>{% avatar hubot size=100 %}</span>



{% for file in site.static_files %}
  {{file.name}}<br>
{% endfor %}


{% for project in site.data.projects %}
  {% capture my_variable %}{{project.name}}{% endcapture %}
  
  {% include image.html url="http://www.google.com" max-width="230px" file="/assets/img/photo78.jpg" caption=my_variable %}

{% endfor %}

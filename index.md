---
title: "QMK Monthly"
layout: default
---

{% for issue in site.issues reversed limit:1 %}
<h3><a href="{{ issue.url }}">{{ issue.title }}</a></h3>
<p>{{ issue.content | markdownify }}</p>
{% endfor %}

{% for issue in site.issues reversed offset:1 %}
<h3><a href="{{ issue.url }}">{{ issue.title }}</a></h3>
{% endfor %}

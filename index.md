---
title: "QMK Monthly"
layout: default
---

{% for issue in site.issues %}
<h1><a href="{{ issue.url }}">{{ issue.title }}</a></h1>
{% if forloop.first == true %}
<p>{{ issue.content | markdownify }}</p>
{% endif %}
{% endfor %}

---
title: "QMK Monthly"
layout: default
---

{% for issue in site.issues limit:1 %}
<h3><a href="{{ issue.url }}">{{ issue.title }}</a></h3>
<p>{{ issue.output }}</p>
{% endfor %}

{% for issue in site.issues offset:1 %}
<h3><a href="{{ issue.url }}">{{ issue.title }}</a></h3>
{% endfor %}

---
title: "QMK Monthly"
layout: default
---

{% for issue in site.issues reversed %}
{% if forloop.first == true %}
# [{{ issue.title }}]({{ issue.url }})
{{ issue.content | markdownify }}

{% else %}
  * [{{ issue.title }}]({{ issue.url }})
{% endif %}
{% endfor %}

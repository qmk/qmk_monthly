---
título: "QMK mensual"
diseño: defecto
---

{% para problema en site.issues revertido %}
{% if forloop.first == verdadero%}
# [{{ problema.titulo }}]({{ problema.url }})

{{ problema.contenido | markdownify }}

## Anterior Problema:

{% más %}
  * [{{ problema.titulo }}]({{ problema.url }})
{% terminara si %}
{% fin de %}

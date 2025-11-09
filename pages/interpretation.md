---
layout: default
title: "Interpretación de Sueños"
tags: [Berajot, Misticismo, Psicología]
permalink: /interpretation/
---

Todo cuanto acontece al hombre en esta realidad física se revela previamente a través de sueños, como expone Rabi Shimon bar Iojai:

_“Treinta días antes de que una nación se transforme en potencia o deba enfrentar alguna desgracia, los niños predicen el evento (como cuando, de modo aparentemente casual, citan alguna frase o versículo que aluda a un hecho inesperado), o a veces la gente más simple lo predice, o incluso los pájaros, a través de conductas extrañas. Pero nadie presta atención, pues nadie comprende tales mensajes. Cuando la nación en cuestión es meritoria, de lo Alto comunican el eventual hecho (a través de sueños) a los líderes virtuosos de la generación para que difundan la advertencia; y así, cuando la gente toma conocimiento de la eventual desgracia retornan al Creador”_ (Zohar, parte II, 6b).

Este diccionario debe priorizar analizar el día antes de interpretar. Los días son en base al calendario judío, que son meses fijados en base al ciclo lunar escritos en el siguiente post:


[Calendario]({% post_url 2025-11-02-calendario-dream %})


### Psicología en la interpretación judía

Sigmund Freud, estudió los sueños, y decia que tienen un lenguaje propio, y son los arquetipos, las imágenes simbólicas, que significan lo mismo o universalmente o en un grupo dado.

Ese concepto es el que Freud denomina lo inconsciente, y que luego, Carl Jung rebautizó como inconsciente personal, denominación que obedece al hecho de que procede de la experiencia personal adquirida, nata, y como tal es propia y específica de cada individuo.

En su _Die Traumdeutung (“Interpretación de los Sueños”)_ en una nota al pie, el autor cita una edición del año 1848 de la obra de **Rabi Shlomó Almoli**, _Pitrón Jalomot_ (literalmente, “Interpretación de los Sueños”), publicada por primera vez bajo el título _Mefasher Jalmin_.

Y estas son las fuentes que usamos para estudio.



## Posts

<ul>
  {% for post in site.posts %}

    {% if post.category == 'sueños' %}
      <li>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}

  {% endfor %}
</ul>

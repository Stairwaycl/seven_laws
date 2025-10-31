---
layout: post
title:  "Un hombre se casa"
categories: hombres
authors: [Rabí Shalom Arush]
references: [En el Jardín de la Paz]
---

Este es el primer mapa conceptual en el que organizamos el estudio de conceptos de lo más general a lo más particular con respecto a _Qué es ser hombre_


<div style="border-radius: 8px; box-shadow: rgba(63, 69, 81, 0.16) 0px 2px 8px 0px; height: 0px; margin-bottom: 0.9em; margin-top: 1.6em; overflow: hidden; padding-bottom: 0px; padding-top: 100%; position: relative; width: 100%; will-change: transform;">
  <iframe allow="fullscreen" allowfullscreen="allowfullscreen" loading="lazy" src="https://www.canva.com/design/DAGyy5lmbso/DH0_jg7E4B1dtqvIbQYmKQ/view?embed" style="border: none; height: 100%; left: 0; margin: 0; padding: 0; position: absolute; top: 0; width: 100%;">
  </iframe>
</div>
<a href="https://www.canva.com/design/DAGyy5lmbso/DH0_jg7E4B1dtqvIbQYmKQ/view?utm_content=DAGyy5lmbso&amp;utm_campaign=designshare&amp;utm_medium=embeds&amp;utm_source=link" rel="noopener" target="_blank">Estudio de Torá Ser Hombre</a>

Iremos actualizando.

{% if page.authors or page.references %}
<div class="post-references mt-5 pt-3 border-top">
    <h3>Referencias</h3>

    {% if page.authors %}
    <p class="small">
        <strong>Sabios mencionados:</strong>
        {% for autor in page.authors %}
            {{ autor }}{% unless forloop.last %}, {% endunless %}
        {% endfor %}
    </p>
    {% endif %}

    {% if page.references %}
    <p class="small">
        <strong>Fuentes del Texto:</strong>
        {% for libro in page.references %}

            <a href="/bibliography/#{{ libro | slugify }}" title="Ver detalles en la Bibliografía Central">
                {{ libro }}
            </a>{% unless forloop.last %}, {% endunless %}
        {% endfor %}
    </p>
    {% endif %}

</div>
{% endif %}

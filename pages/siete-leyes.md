---
layout: default
permalink: /siete-leyes/
---
# 📜 Las Siete Leyes de Noaj
1. Prohibición de la Idolatría

2. Prohibición de la Blasfemia

3. Prohibición del Asesinato

4. Prohibición de las Relaciones Sexuales Ilícitas

5. Prohibición del Robo

6. Prohibición de Comer la Carne de un Animal Vivo

7. Mandamiento de Establecer Tribunales de Justicia

## Posts
<div>

<ul>
  {% for post in site.posts %}

    {% if post.category == 'siete-leyes' %}
      <li>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}

  {% endfor %}
</ul>

</div>

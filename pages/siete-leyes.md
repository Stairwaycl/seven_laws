---
layout: default
---
# Fundamentos del judaísmo según Maimónides.

<div>
    {% for post in site.posts %}

      {%- assign post_date = post.date | date: "%s" -%}
      {%- assign current_date = 'now' | date: "%s" -%}

      {% comment %}
        *** AÑADIR LA CONDICIÓN DE FILTRADO AQUÍ *** Usamos 'contains' ya que la propiedad 'categories' puede ser una lista.
      {% endcomment %}
      {% if post_date <= current_date and post.categories contains "siete-leyes" and post.slug == "fundamentos" %}

        <div class="col">
          <div>
            <div>

              <h6 class="card-subtitle mb-2 text-muted">
                {{ post.date | date: "%d %b %Y" }}
              </h6>

              <h5 class="card-title">{{ post.title }}</h5>

              <p class="card-text">
                {% comment %} Si quieres el contenido COMPLETO, usa '.content' {% endcomment %}
                {{ post.content }}
              </p>

            </div>
          </div>
        </div>

        {% comment %}
          *** DETENER EL BUCLE DESPUÉS DE ENCONTRAR EL POST ***
          Como solo quieres UNO, usa 'break' para optimizar el rendimiento.
        {% endcomment %}
        {% break %}

      {% endif %}
    {% endfor %}

</div>

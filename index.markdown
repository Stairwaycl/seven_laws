---
# IMPORTANTE: Con esto le dices a Jekyll que use la configuración de paginación.
layout: default
pagination:
  enabled: true
---


<div class="container my-5">

  <div class="row row-cols-1 g-4">

    {% for post in paginator.posts %}

      {%- assign post_date = post.date | date: "%s" -%}
      {%- assign current_date = 'now' | date: "%s" -%}

      {% if post_date <= current_date %}

        <div class="col">
          <div class="card h-100 shadow-sm">
            <div class="card-body">

              <h6 class="card-subtitle mb-2 text-muted">
                {% assign display_date = post.date %}
                {% if post.last_modified_at %}
                  {% assign display_date = post.last_modified_at %}
                {% endif %}

                {{ display_date | date: "%d %b %Y" }}
              </h6>

              <h5 class="card-title">{{ post.title }}</h5>

              <p class="card-text">{{ post.excerpt }}</p>

            </div>
            <div class="card-footer border-0">
                <a href="{{ post.url | relative_url }}" class="btn btn-primary">Leer más</a>
            </div>
          </div>
        </div>

      {% endif %}
    {% endfor %}
  </div>
</div>

<div class="container my-4">
    <div class="d-flex justify-content-between align-items-center">

        {% if paginator.previous_page %}
            <a class="btn btn-outline-secondary" href="{{ paginator.previous_page_path | relative_url }}">
                &larr; Recientes
            </a>
        {% else %}
            <span class="btn btn-outline-secondary disabled">&larr; Recientes</span>
        {% endif %}

        <span class="text-muted">
            Página {{ paginator.page }} de {{ paginator.total_pages }}
        </span>

        {% if paginator.next_page %}
            <a class="btn btn-outline-secondary" href="{{ paginator.next_page_path | relative_url }}">
                Antiguos &rarr;
            </a>
        {% else %}
            <span class="btn btn-outline-secondary disabled">Antiguos &rarr;</span>
        {% endif %}

    </div>
</div>

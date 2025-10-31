---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---


<div class="container my-5">

  <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">

    {% for post in site.posts %}

      {%- assign post_date = post.date | date: "%s" -%}
      {%- assign current_date = 'now' | date: "%s" -%}

      {% if post_date <= current_date %}

        <div class="col">
          <div class="card h-100 shadow-sm">
            <div class="card-body">

              <h6 class="card-subtitle mb-2 text-muted">
                {{ post.date | date: "%d %b %Y" }}
              </h6>

              <h5 class="card-title">{{ post.title }}</h5>

              <p class="card-text">{{ post.excerpt }}</p>

            </div>
            <div class="card-footer bg-white border-0">
                <a href="{{ post.url }}" class="btn btn-primary">Leer más</a>
            </div>
          </div>
        </div>

      {% endif %}
    {% endfor %}
  </div>
</div>

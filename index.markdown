---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<ul>
  {% for post in site.posts %}


    {%- assign post_date = post.date | date: "%s" -%}

    {%- assign current_date = 'now' | date: "%s" -%}


    {% if post_date <= current_date %}

      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>

        <div class="card" style="width: 18rem;">
          <div class="card-body">
            <h5 class="card-title">{{post.title}}</h5>

            <p class="card-text">{{post.excerpt}}</p>
            <a href="{{ post.url }}">Leer más</a>
          </div>
        </div>
      </li>
    {% endif %}
  {% endfor %}
</ul>

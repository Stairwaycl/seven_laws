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
      </li>

    {% endif %}



  {% endfor %}
</ul>

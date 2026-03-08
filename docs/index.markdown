---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
show_on_home: false
---


# On sex and pleasure experiments

Welcome! Here you can find some relevant posts and pages ;)

## Posts

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

## Pages

<ul>
{% for page in site.pages %}
  {% if page.title and page.show_on_home == true %}
  <li>
    <a href="{{ page.url | relative_url }}">{{ page.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>
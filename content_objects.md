---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---


# Content-Objects
Work in progress

<ul>
{% for cobject in site.content_objects %}
  <li>
    <a href="{{ cobject.url }}">
      {{ cobject.name }}
    </a>
  </li>
{% endfor %}
</ul>

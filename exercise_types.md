---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---


# Exercise-Types
<ul>
{% for etype in site.exercise_types %}
  <li>
    <a href="/models/{{ etype.name }}.html">
      {{ etype.title }}
    </a>
  </li>
{% endfor %}
</ul>

---
layout: default
title: Physical Science Standards
---

<div>
  {%- if site.edu-standards.size > 0 -%}
    <h2 class="post-list-heading">{{ page.list_title | default: "Physical Science Standards" }}</h2>
    <ul class="post-list">
      {%- for lesson in site.edu-standards -%}
      <li>
        <h3>
          <a class="post-link" href="{{ lesson.url | relative_url }}">
            {{ lesson.title | escape }}
          </a>
        </h3>
        {%- if site.show_excerpts -%}
          {{ lesson.excerpt }}
        {%- endif -%}
      </li>
      {%- endfor -%}
    </ul>
  {%- endif -%}
</div>
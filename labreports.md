---
layout: default
Instructional Planning Resource
---
<div class="home">
	{%- if site.labreports.size > 0 -%}
    <h2 class="post-list-heading">{{ page.list_title | default: "Lab Reports" }}</h2>
    <ul class="post-list">
      {%- for lesson in site.labreports -%}
      <li>
        <h3>
          <a class="post-link" href="{{ lesson.url | relative_url }}">
            {{ lesson.title | escape }}
          </a>
        </h3>
        
      </li>
      {%- endfor -%}
    </ul>
  {%- endif -%}
</div>
---
layout: default
---

# How to handle assets hosted elsewhere: a demonstration

## Simple approach: code within page content

<ul>
{% for page in site.simple %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

## Intermediate approach: embed code in front matter; Liquid tag in layout

<ul>
{% for page in site.intermediate %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

## More advanced approach: source link in front matter; code with Liquid tag in layout

### Audio
<ul>
{% for page in site.audio %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

### Images
<ul>
{% for page in site.images %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

### Video
<ul>
{% for page in site.video %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

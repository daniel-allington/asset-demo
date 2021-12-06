---
layout: default
---

# How to handle assets hosted elsewhere: a demonstration

## Simple approach: embed code or IMG tag within page content

<ul>
{% for page in site.simple %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

## Intermediate approach: unedited embed code in page front matter; Liquid tag in layout file

<ul>
{% for page in site.intermediate %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

## More advanced approach: source URL in page front matter; edited embed code or IMG tag with Liquid tag in layout file

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

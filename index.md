---
layout: default
---

## Simple approach: code within page content

<ul>
{% for page in site.simple %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

## More advanced approach: code in layout; source link in front matter

Audio
<ul>
{% for page in site.audio %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

Images
<ul>
{% for page in site.images %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

Video
<ul>
{% for page in site.video %}
<li><a href = "{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

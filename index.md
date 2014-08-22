---
layout: archive
permalink: /
title: "A Designer’s Faux Pas"
excerpt: "Making stuff one mmistake at a time."
image:
  feature: 
id: home
---

### Paper by 53

<div class="tiles">
{% for post in site.categories.mastering-paper limit:4 %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

---

### Latest Articles

<div class="tiles">
{% for post in site.categories.articles limit:4 %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

---

### Latest PaperFaces

<ul class="th-grid-full">
{% for post in site.categories.paperfaces limit:8 %}
  <li><a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}"><img src="{{ site.url }}/images/{{ post.image.thumb }}" alt="thumbnail image"></a></li>
{% endfor %}
</ul>
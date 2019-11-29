---
layout: default
work: true
main: true
title: "Bioinformatics"
description: 생물정보학에 관한 글을 올려요.
project-header: true
header-img: img/about.jpg
---

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.bioinformatics == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>


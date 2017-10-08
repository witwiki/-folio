---
layout: page
permalink: /resume/
title: resume
---

<ul class="post-list">
{% for pos in site.resume reversed %}
    <li>
        <h2><a class="pos-title" href="{{ pos.url | prepend: site.baseurl }}">{{ pos.title }}</a></h2>
        <p class="post-meta">{{ pos.date | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>
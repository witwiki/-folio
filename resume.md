---
layout: page
permalink: /resume/
title: resume
---

<ul class="post-list">
{% for pos in site.resume reversed %}
    <li>
        <h2><a class="pos-title" href="{{ pos.url | prepend: site.baseurl }}">{{ pos.title }}</a>
        &nbsp;&nbsp;<a class="pos-title" href="vstudios.space">{{ pos.company }}</a></h2>
        <br>
        <br>
        <p class="post-meta">{{ pos.date | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>
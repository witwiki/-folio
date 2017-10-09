---
layout: page
permalink: /resume/
title: resume
---

<ul class="post-list">
{% for pos in site.resume reversed %}
    <li>
        <h2><a class="page-heading" href="{{ pos.url | prepend: site.baseurl }}">{{ pos.title }}&nbsp;&nbsp;-</a>
        <a class="page-heading" href="{{ pos.siteUrl }}">&nbsp;&nbsp;{{ pos.company }}</a></h2>
        
        <p class="post-meta">{{ pos.fromDate | date: '%B %-d, %Y' }}&nbsp;-&nbsp;{{ pos.toDate | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>
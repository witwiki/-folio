---
layout: page
permalink: /resume/
title: resume
---

<ul class="post-list">
{% for pos in site.resume reversed %}
    <li>
        <h2><a class="page-heading" href="{{ pos.url | prepend: site.baseurl }}">{{ pos.title }}::</a>
        <a class="page-heading" href="{{ pos.siteUrl }}">{{ pos.company }}</a></h2>
        <p class="post-meta">{{ pos.fromDate | date: '%B %-d, %Y' }}&nbsp;-&nbsp;{{ pos.toDate | date: '%B %-d, %Y' }}</p>
      </li>
      <hr>
{% endfor %}
</ul>
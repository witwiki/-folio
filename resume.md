---
layout: page
permalink: /resume/
title: resume
---

<ul class="post-list">
{% for pos in site.resume reversed %}
    <li>
        <h2><a class="page-heading" href="{{ pos.url | prepend: site.baseurl }}">{{ pos.title }}</a>
        &nbsp;&nbsp;-&nbsp;&nbsp;<a class="post-title" href="{{ pos.siteUrl }}">{{ pos.company }}</a></h2>
        <br>
        <p class="post-meta">{{ pos.fromDate | date: '%B %-d, %Y' }}&nbsp;-&nbsp;{{ pos.toDate | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>
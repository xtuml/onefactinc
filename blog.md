---
layout: default
title: Blog
description: Articles and notes from One Fact on xtUML, systems modeling, and engineering.
permalink: /blog/
---

<section class="page-hero">
  <div class="container">
    <p class="eyebrow">ONE FACT INSIGHTS</p>
    <h1>Articles &amp; notes.</h1>
    <p class="hero-lede">Ideas, technical notes, announcements, and stories from the One Fact archive.</p>
  </div>
</section>
<section class="section">
  <div class="container">
    <div class="article-list">
      {% assign articles = site.articles | sort: "title" %}
      {% for article in articles %}
      <article class="article-list-item">
        <h2><a href="{{ article.url | relative_url }}">{{ article.title | escape }}</a></h2>
        {% if article.description %}<p>{{ article.description | escape }}</p>{% endif %}
        <a href="{{ article.url | relative_url }}">Read article →</a>
      </article>
      {% endfor %}
    </div>
  </div>
</section>

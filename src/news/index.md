---
title: News
nav:
  order: 3
---

These are latest Articles from [Rawsta]{.rawsta} :

<div class="stack">

{% for entry in collections.news %}

  <article class="news">
    <h2 class="news__title"><a href="{{ entry.url }}">{{ entry.data.title }}</a></h2>
    <p class="news__meta">{{ entry.date | date("Do MMMM YYYY") }}</p>
  </article>
{% endfor %}

</div>

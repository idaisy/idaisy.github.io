---
layout: default
title: Planet Money
permalink: /PlanetMoney/
---

## Planet Money

<div class="home">

  <ul class="post-list">
{% for post in site.posts %}
  {% for tag in post.tags %}
    {% if tag == "Planet Money" %}
      <li>
        <!--<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>-->
        <span class="post-meta">{{ post.date | date: "%Y-%m-%d,%A" }}</span>

        <h1>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h1>
      </li>
    {% break %}
    {% endif %}
  {% endfor %}
{% endfor %}
  </ul>

</div>

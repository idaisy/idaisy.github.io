---
layout: default
title: How I Built This
permalink: /Built/
---

How I Built This 是 NPR 旗下的一档关于创业故事的节目

<div class="home">

  <ul class="post-list">
{% for post in site.posts %}
  {% for tag in post.tags %}
    {% if tag == "Built" %}
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

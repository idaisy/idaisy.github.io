---
layout: default
title: How I Built This
permalink: /Built/
---

![](http://media.npr.org/assets/img/2016/08/31/hibt_podcast_tile_sq-8d9498b292dc7a759bf4b7fc776dfe0e4c09da68-s300-c85.png)

How I Built This 是 NPR 旗下的一档关于[innovators]{创新者}、[entrepreneurs]{创业者}、[idealists]{理想主义者}及他们创建的[movements]{运动}的节目。

> From NPR, it's HOW I BUILT THIS, a show about innovators, entrepreneurs, idealists and the stories behind the movements they built.

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

---
layout: default
title: Planet Money
permalink: /PlanetMoney/
---
![](http://media.npr.org/assets/img/2015/12/18/planetmoney_sq-c7d1c6f957f3b7f701f8e1d5546695cebd523720-s300-c85.jpg)

Planet Money 是 NPR 旗下的一档日常经济学相关的Podcast. 非常有趣味.

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

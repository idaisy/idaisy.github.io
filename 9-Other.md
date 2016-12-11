---
layout: default
title: Other
permalink: /Other/
---

## Other

<div class="home">

  <ul class="post-list">
{% for post in site.posts %}
 {% if post.tags == empty %}
      <li>
        <!--<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>-->
        <span class="post-meta">{{ post.date | date: "%Y-%m-%d,%A" }}</span>

        <h1>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h1>
      </li>
 {% endif %}
{% endfor %}
  </ul>

</div>

---
layout: default
---


在这里, 我会定期的选取一些国外好的Podcast, 并把里面遇到的生词标注好, 方便大家做预习和听后校对.

目前主要在更新[Planet Money](/PlanetMoney/). 如果你也想加入进来, 欢迎邮件联系我.

本站可以通过[RSS订阅]({{ "/feed.xml" | prepend: site.baseurl }}).

## 所有条目

<div class="home">

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%Y-%m-%d,%A" }}</span>

        <h1>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h1>
      </li>
    {% endfor %}
  </ul>

</div>

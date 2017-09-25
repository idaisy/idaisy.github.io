---
layout: default
---

- 翻译引进国外创新创业、经济相关的播客(Podcast)。
- 目标不是向听众提供完整的字幕，而是为听众提供必要的背景及语言信息，从而使得他们能够听到原汁原味的国外的音频节目。
- 目前主要涵盖的节目范围:
	- Planet Money, NPR旗下的一档关于经济常识的节目
	-	How I Built This，NPR旗下的一档关于创业故事的节目
	-	99% Invisible
	-	Radiolab

本站可以通过[RSS订阅]({{ "/feed.xml" | prepend: site.baseurl }}).

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

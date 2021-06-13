---
layout: default
title: 文章
---

# 文章列表

<p class="message" style="background-color: #e64980;">
  👋 以下的推送文章按照年月进行排序
</p>

{% assign postsByYearMonth = site.posts | group_by_exp: "post", "post.date | date: '%B %Y'" %}
{% for yearMonth in postsByYearMonth %}
  <h2>{{ yearMonth.name }}</h2>
  <ul>
    {% for post in yearMonth.items %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

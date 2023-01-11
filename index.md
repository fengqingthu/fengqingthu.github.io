---
layout: page
list_title: ' '
---

因为厌倦了微信没休止的审查，我把个人随笔都搬到了github上，也以防某天QQ空间下线，小时候的东西就都丢了。

<br />

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
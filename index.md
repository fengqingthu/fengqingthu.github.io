---
layout: page
list_title: ' '
---

一直想要做一个自己的网站用来堆东西，迟迟没有契机。跨年时厌倦了微信没休止的审查，我决定把个人随笔都搬到了github上，也以防某天QQ空间下线，小时候的东西就都丢了。打算慢慢地有时间把速写和音乐都挪过来，让它热闹一点点。

<br />

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
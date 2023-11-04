---
layout: page
list_title: ' '
---

人生梦想是财务自由以后当个作家，分享自己的personal essays，于是做了现在这个早期存储的地方。

<br />

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
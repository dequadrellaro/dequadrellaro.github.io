---
permalink: /blog/
---

<div align="center" style="margin-top: 1.5em; margin-bottom: 1.5em;">
  <img src="/000055 (copy).jpg" alt="picture" width="75%">
</div>
 
<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="post-list-date">{{ post.date | date: "%B %-d, %Y" }}</span>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
 

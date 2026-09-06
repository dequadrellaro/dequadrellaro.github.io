---
permalink: /blog/
---
 
<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="post-list-date">{{ post.date | date: "%B %-d, %Y" }}</span>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
 

---
permalink: /blog/
---

<div align="center" style="margin-top: 1.5em; margin-bottom: 1.5em;">
  <img src="/assets/images/photo:blog.jpg" alt="picture" width="75%">
</div>


<p><a href="{{ "/feed.xml" | absolute_url }}">Subscribe via RSS</a></p>

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="post-list-date">{{ post.date | date: "%B %-d, %Y" }}</span>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
 
<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="post-list-date">{{ post.date | date: "%B %-d, %Y" }}</span>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
 

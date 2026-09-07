---
permalink: /blog2/
---

<div align="center" style="margin-top: 1.5em; margin-bottom: 1.5em;">
  <img src="/assets/images/photo:miscellanea.jpg" alt="picture" width="75%">
</div> 


<p style="text-align: center;"><a href="{{ "/feed.xml" | absolute_url }}" class="rss-link">Subscribe via RSS</a> | <a href="/archive" class="rss-link" >Blog Archive</a> </p>


<!--  <ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="post-list-date">{{ post.date | date: "%B %-d, %Y" }}</span>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul> --->
 
{% for post in site.posts limit:5 %}
<article class="post-entry">
  <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
  {{ post.content }}
</article>
<hr class="post-divider">
{% endfor %}

<!--  A full list of past posts can be found in the [archive](/archive). --->

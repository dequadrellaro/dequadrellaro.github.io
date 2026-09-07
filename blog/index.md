
<div align="center" style="margin-top: 1.5em; margin-bottom: 1.5em;">
  <img src="/assets/images/photo:miscellanea.jpg" alt="picture" width="75%">
</div> 

<p style="text-align: center;"><a href="{{ "/feed.xml" | absolute_url }}" class="rss-link">Subscribe via RSS</a> | <a href="/archive" class="rss-link" >Blog Archive</a> </p>

{% assign posts = site.posts | offset: 0 | limit: 5 %}
{% for post in posts %}
<article class="post-entry">
  <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
  {{ post.content }}
</article>
<hr class="post-divider">
{% endfor %}

{% if site.posts.size > 5 %}
<nav class="pagination"><a href="/blog/page2/">Older posts &rarr;</a></nav>
{% endif %}

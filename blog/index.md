markdown
---
---

<p class="rss-link-wrapper" style="text-align: center;"><a href="{{ "/feed.xml" | absolute_url }}" class="rss-link">Subscribe via RSS</a></p>

{% for post in paginator.posts %}
<article class="post-entry">
  <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
  {{ post.content }}
</article>
<hr class="post-divider">
{% endfor %}

<nav class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path | relative_url }}">&larr; Newer posts</a>
  {% endif %}
  {% if paginator.previous_page and paginator.next_page %} | {% endif %}
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path | relative_url }}">Older posts &rarr;</a>
  {% endif %}
</nav>

A full list of past posts can be found in the [archive](/archive).

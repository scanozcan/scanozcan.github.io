---
layout: page
title: News & Blog
permalink: /blog/
---

{% assign news_posts = site.posts | where: "categories", "news" %}
{% if news_posts.size > 0 %}
<h2 id="news">News</h2>

<div class="publications-grid">
  {% for post in news_posts %}
  <div class="publication-item">
    <div class="publication">
      <div class="pub-title">
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        {% if post.doi %}
          <a href="{{ post.doi }}" class="pub-icon-link" title="DOI">
            <i class="ai ai-doi"></i>
          </a>
        {% endif %}
      </div>
      <div class="pub-venue">{{ post.date | date: "%b %-d, %Y" }}</div>
    </div>
  </div>
  {% endfor %}
</div>
{% endif %}

{% assign blog_posts = site.posts | where: "categories", "general" %}
{% if blog_posts.size > 0 %}
<h2 id="blog-posts">Blog Posts</h2>

<div class="publications-grid">
  {% for post in blog_posts %}
  <div class="publication-item">
    <div class="publication">
      <div class="pub-title">
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </div>
      <div class="pub-venue">{{ post.date | date: "%b %-d, %Y" }}</div>
    </div>
  </div>
  {% endfor %}
</div>
{% endif %}

{% if site.posts.size == 0 %}
  <p>No posts yet. Check back soon!</p>
{% endif %}

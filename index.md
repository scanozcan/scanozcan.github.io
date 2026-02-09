---
layout: home
title: About
permalink: /
---

# Selahattin Can Özcan

### Cancer Biology | Forward Genomics | Regeneration | Data Analysis

<div class="bio-section">
  <div class="bio-text" markdown="1">

I am currently a researcher at the **[SRSP Lab](https://woappilab.com)** at **[Columbia University](https://www.columbia.edu)**, where I use highly multiplexed CRISPR screens to investigate mammalian regeneration in skin wounds. My expertise also spans cancer biology & metabolism, chromosomal instability, proximity proteomics, and the epigenetic regulation of stem cell differentiation.

I love fooling around with plasmids and DNA sequences! I also enjoy exploring diverse datasets. Looking ahead, I aim to apply evolutionary game theory to understand cellular decision-making and cell-cell communication in cancer and tissue biology.

  </div>
  <img src="{{ '/assets/images/profile.png' | relative_url }}" alt="Profile Photo" class="profile-photo">
</div>

{% assign news_posts = site.posts | where: "categories", "news" %}
{% if news_posts.size > 0 %}
## News

<div class="publications-grid">
  {% for post in news_posts limit:2 %}
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
<p class="view-all"><a href="{{ '/blog/#news' | relative_url }}">View all &rarr;</a></p>
{% endif %}

{% assign blog_posts = site.posts | where: "categories", "general" %}
{% if blog_posts.size > 0 %}
## Recent Blog Posts

<div class="publications-grid">
  {% for post in blog_posts limit:4 %}
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
<p class="view-all"><a href="{{ '/blog/#blog-posts' | relative_url }}">View all &rarr;</a></p>
{% endif %}

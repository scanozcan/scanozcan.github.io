---
layout: home
title: About
permalink: /
---

# Selahattin Can Özcan

### Cancer Biology | Functional Genomics & Proteomics | Cell Decision-Making

<div class="bio-section">
  <div class="bio-text" markdown="1">

I'm a biologist trying to understand how cells make decisions — in cancer, and in tissue repair. Currently at **[Columbia University](https://www.columbia.edu)**<!-- at the **[SRSP Lab](https://woappilab.com)** -->, I design and use cell-type multiplexed CRISPR screens to dissect the genetic programs driving regeneration in mammalian skin wound healing. My research has also moved through cancer metabolism, chromosomal instability, and epigenetic regulation of stem cell differentiation — and I've built computational tools along the way to find better ways to analyze the genomic locus proteomics data.

I'm interested in the molecular logic of cell decision-making — the pathways and connections that determine why a cell chooses one fate over another, why the same perturbation leads to different outcomes in different tissues. Evolutionary game theory appeals to me as a formal framework for thinking about these decisions. What I enjoy most is the moment scattered data — screen hits, omics signals — start to form a coherent biological story.

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
        {% if post.github %}
          <a href="{{ post.github }}" class="pub-icon-link" title="GitHub" target="_blank" rel="noopener">
            <i class="fab fa-github"></i>
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

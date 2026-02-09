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
{% endif %}

<div style="margin-top: 40px;" markdown="1">

**Office**: Russ Berrie Pavilion, Room 606<br>
**Address**: 1150 St. Nicholas Ave, New York, NY 10032

</div>

<!-- Social Links - Now with your custom Bluesky SVG -->
<div style="margin-top: 20px; clear: both; display: flex; gap: 20px; flex-wrap: wrap; align-items: center; justify-content: center;" class="icon-container">
  
  <!-- Email - Font Awesome -->
  <a href="mailto:so2716@cumc.columbia.edu" style="text-decoration: none; color: inherit;" title="Email">
    <i class="fas fa-envelope"></i>
  </a>
  
  <!-- Google Scholar - Academicons -->
  <a href="https://scholar.google.com.tr/citations?user=VIo4te8AAAAJ&hl=en" style="text-decoration: none; color: inherit;" title="Google Scholar">
    <i class="ai ai-google-scholar"></i>
  </a>
  
  <!-- ORCID - Academicons -->
  <a href="https://orcid.org/0000-0003-1733-4288" style="text-decoration: none; color: inherit;" title="ORCID">
    <i class="ai ai-orcid"></i>
  </a>
  
  <!-- GitHub - Font Awesome -->
  <a href="https://github.com/scanozcan" style="text-decoration: none; color: inherit;" title="GitHub">
    <i class="fab fa-github"></i>
  </a>
  
  <!-- LinkedIn - Font Awesome -->
  <a href="https://www.linkedin.com/" style="text-decoration: none; color: inherit;" title="LinkedIn">
    <i class="fab fa-linkedin"></i>
  </a>
  
  <!-- Bluesky - Your custom SVG (fixed to inherit color) -->
  <a href="https://bsky.app/profile/ozcansc.bsky.social" style="text-decoration: none; color: inherit;" title="Bluesky">
    <svg width="24" height="24" viewBox="0 0 40 40" fill="currentColor" style="vertical-align: middle;">
      <path d="M11.143 2.153c4.19 3.123 8.703 9.453 10.357 12.85 1.654-3.397 6.167-9.727 10.357-12.85 3.026-2.255 7.924-3.999 7.924 1.552 0 5.55-.637 9.306-1.017 10.64-1.306 4.632-6.064 5.807-10.293 5.091 7.397 1.246 9.276 5.385 5.214 9.524-7.718 7.856-11.09-1.974-11.953-4.49-.161-.46-.232-.677-.232-.492 0-.186-.077.032-.232.491-.862 2.517-4.235 12.347-11.954 4.49-4.061-4.138-2.182-8.27 5.214-9.523-4.229.716-8.986-.466-10.292-5.09-.38-1.335-1.017-9.536-1.017-10.648 0-5.544 4.898-3.8 7.924-1.545Z"/>
    </svg>
  </a>
  
  <!-- Instagram - Font Awesome -->
  <a href="https://www.instagram.com/scanozc?igsh=MXVlYWlmZ2oxNG1iMg%3D%3D&utm_source=qr" style="text-decoration: none; color: inherit;" title="Instagram">
    <i class="fab fa-instagram"></i>
  </a>

  <!-- Spotify - Custom SVG -->
  <a href="https://open.spotify.com/user/cozcan89/playlists" style="text-decoration: none; color: inherit;" title="Spotify">
    <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" style="vertical-align: middle;" class="spotify-icon">
      <path d="M12 0C5.4 0 0 5.4 0 12s5.4 12 12 12 12-5.4 12-12S18.66 0 12 0zm5.521 17.34c-.24.359-.66.48-1.021.24-2.82-1.74-6.36-2.101-10.561-1.141-.418.122-.779-.179-.899-.539-.12-.421.18-.78.54-.9 4.56-1.021 8.52-.6 11.64 1.32.42.18.479.659.301 1.02zm1.44-3.3c-.301.42-.841.6-1.262.3-3.239-1.98-8.159-2.58-11.939-1.38-.479.12-1.02-.12-1.14-.6-.12-.48.12-1.021.6-1.141C9.6 9.9 15 10.561 18.72 12.84c.361.181.54.78.241 1.2zm.12-3.36C15.24 8.4 8.82 8.16 5.16 9.301c-.6.179-1.2-.181-1.38-.721-.18-.601.18-1.2.72-1.381 4.26-1.26 11.28-1.02 15.721 1.621.539.3.719 1.02.419 1.56-.299.421-1.02.599-1.559.3z"/>
    </svg>
  </a>

</div>

<div style="clear: both;"></div>


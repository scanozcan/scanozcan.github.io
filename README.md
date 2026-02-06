# Academic Website

A minimal academic website built with Jekyll and hosted on GitHub Pages.

## Quick Start

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler (`gem install bundler`)

### Local Development

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/academic-website.git
   cd academic-website
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Run the local server:
   ```bash
   bundle exec jekyll serve
   ```

4. Open http://localhost:4000 in your browser

## Customization

### Site Configuration

Edit `_config.yml` to update:
- Site title and description
- Your name and email
- Social media links
- Navigation pages

### Homepage

Edit `index.md` to update:
- Your bio and introduction
- Research interests
- Education
- News/updates
- Contact information

Replace `assets/images/profile.jpg` with your photo.

### Publications

Edit `_data/publications.yml` to add/modify publications. Each publication can have:
- `title`: Paper title
- `authors`: Author list
- `venue`: Conference/journal name
- `year`: Publication year
- `type`: conference, journal, workshop, or preprint
- `links`: pdf, doi, code, slides
- `highlight`: true to feature the publication

### Blog Posts

Add new posts to `_posts/` with the format `YYYY-MM-DD-title.md`.

Each post needs front matter:
```yaml
---
layout: post
title: "Post Title"
date: YYYY-MM-DD
categories: category-name
---
```

## Deployment to GitHub Pages

1. Create a new repository on GitHub
2. Push your code:
   ```bash
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```
3. Go to Settings > Pages > Source: Deploy from branch (main)
4. Your site will be live at `https://yourusername.github.io`

### Custom Domain (Optional)

1. Add a `CNAME` file with your domain
2. Configure DNS settings with your domain provider

## File Structure

```
├── _config.yml           # Site configuration
├── _data/
│   └── publications.yml  # Publications data
├── _includes/
│   └── publication.html  # Publication template
├── _layouts/
│   └── publications.html # Publications page layout
├── _posts/               # Blog posts
├── _sass/
│   └── custom.scss       # Custom styles
├── assets/
│   ├── css/
│   │   └── style.scss    # Main stylesheet
│   └── images/           # Images
├── index.md              # Homepage
├── publications.md       # Publications page
├── blog.md               # Blog listing
├── Gemfile               # Dependencies
└── README.md             # This file
```

## License

MIT License - feel free to use this template for your own academic website.

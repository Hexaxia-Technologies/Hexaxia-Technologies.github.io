# Hexaxia Technologies Blog

Official technical blog for Hexaxia Technologies, powered by GitHub Pages and Jekyll.

**Live Site**: https://hexaxia-technologies.github.io

## Blog Structure

```
.
├── _config.yml           # Jekyll configuration
├── _posts/               # Blog posts (YYYY-MM-DD-title.md)
├── _authors/             # Author profiles
├── _layouts/             # Custom layouts (optional)
├── index.md              # Homepage
├── about.md              # About page
└── Gemfile               # Ruby dependencies
```

## Writing a New Blog Post

1. Create a new file in `_posts/` with the format: `YYYY-MM-DD-title.md`

2. Add front matter at the top:

```yaml
---
layout: post
title: "Your Post Title"
date: 2026-01-23 12:00:00 -0500
categories: [category1, category2]
tags: [tag1, tag2, tag3]
author: Author Name
excerpt: "Brief description for previews and SEO"
---
```

3. Write your content in Markdown below the front matter

4. Commit and push - GitHub Pages will automatically build and publish

## Adding a New Author

Create a file in `_authors/` named `author-slug.md`:

```yaml
---
short_name: author-slug
name: Full Name
position: Job Title
github: https://github.com/username
website: https://personal-site.com
---

Short bio about the author.
```

## Local Development

To test the blog locally before publishing:

```bash
# Install dependencies
bundle install

# Run local server
bundle exec jekyll serve

# View at http://localhost:4000
```

## RSS Feed

RSS feed is automatically generated at `/feed.xml` via the `jekyll-feed` plugin.

## Deployment

GitHub Pages automatically builds and deploys when you push to the `main` branch. No manual deployment needed.

## Integration with hexaxia.tech

This blog's RSS feed is aggregated into the main Hexaxia Technologies website at https://hexaxia.tech/blog using the blog aggregation system.

The RSS feed URL for integration: `https://hexaxia-technologies.github.io/feed.xml`

## GitHub Pages Settings

Ensure your repository settings have:
- Pages source: `main` branch, `/ (root)` folder
- Custom domain (optional): Can configure if desired
- Enforce HTTPS: Enabled

## Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Jekyll Themes](https://jekyllrb.com/docs/themes/)

# Instant History Blog

This is Michael Morisy's personal blog built with Jekyll and hosted on GitHub Pages.

## Quick Start

### Writing a New Post

1. Create a new file in the `_posts` folder
2. Name it using the format: `YYYY-MM-DD-post-title.md`
3. Add the following front matter at the top:

```yaml
---
layout: post
title: "Your Post Title"
subtitle: "Optional subtitle"
date: 2024-01-15 10:00:00
tags: [tag1, tag2]
---
```

4. Write your content using Markdown

### Markdown Features

This blog supports enhanced markdown features:

- **GitHub Flavored Markdown**: Tables, strikethrough, task lists
- **Code syntax highlighting**: Use triple backticks with language identifier
- **Emojis**: Type `:emoji_name:` (e.g., `:smile:`)
- **@mentions**: Link to GitHub users with `@username`
- **Footnotes**: Use `[^1]` for footnote markers

Example:
```markdown
This is some text with a footnote[^1].

[^1]: This is the footnote content.
```

### Local Development

1. Install Ruby and Bundler
2. Run `bundle install` to install dependencies
3. Run `bundle exec jekyll serve` to start local server
4. Visit `http://localhost:4000`

### Deployment

The site automatically deploys to GitHub Pages when you push to the main branch.

## Features

- **SEO Optimization**: Automatic meta tags and Open Graph data
- **Reading Time**: Shows estimated reading time for each post
- **Sitemap**: Automatically generated at `/sitemap.xml`
- **RSS Feed**: Available at `/feed.xml`
- **Syntax Highlighting**: Beautiful code blocks with line numbers
- **Social Sharing**: Twitter and Facebook share buttons
- **Comments**: Configured for Staticman (requires setup)

## Configuration

Main settings are in `_config.yml`:
- Site title and description
- Author information
- Social media links
- Google Analytics
- Comment system settings

## Tips

- Use `<!--more-->` in posts to set excerpt break point
- Add `image: /path/to/image.jpg` in front matter for social media previews
- Use `redirect_from: /old-url/` to redirect old URLs
- Posts with future dates won't be published until that date

## Troubleshooting

If the site doesn't update after pushing:
1. Check GitHub Actions tab for build errors
2. Ensure post filenames are correctly formatted
3. Verify front matter YAML is valid
4. Check that post dates aren't in the future
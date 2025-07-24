# NeuvoBlog

A minimalist Jekyll blog with chronological posts and topic-based organization.

## Quick Start

### Writing Posts

1. Create a new file in `_posts/` with format: `YYYY-MM-DD-title.md`
2. Add minimal front matter:
   ```yaml
   ---
   title: "Your Post Title"
   ---
   ```
3. Write your content in Markdown
4. Use `<!--more-->` to separate excerpt from full content

### Adding Categories

Add categories to organize posts by topic:
```yaml
---
title: "Your Post Title"
categories: [technology, culture]
---
```

### Creating Topic Pages

1. Create a file in `_topics/` named `topic-name.md`
2. Use the topic layout:
   ```yaml
   ---
   layout: topic
   title: Topic Name
   topic: topic-name
   description: Brief description
   ---
   ```

## Project Structure

```
├── _posts/          # Blog posts (YYYY-MM-DD-title.md)
├── _topics/         # Topic pages
├── _layouts/        # Page templates
├── assets/css/      # Stylesheets
├── index.html       # Homepage
├── archive.html     # All posts
├── topics.html      # Topic index
└── about.md         # About page
```

## GitHub Pages Deployment

1. Create repository with any name (e.g., `neuvo-blog`)
2. Push all files to the repository
3. Enable GitHub Pages in repository Settings → Pages → Deploy from branch: `main`
4. Access at `https://jbstavers.github.io/neuvo-blog`

## Customization

- Edit `_config.yml` for site settings
- Modify CSS in `assets/css/style.css`
- Create new layouts in `_layouts/`
- Add pages at root level

## Writing Tips

- Keep front matter minimal
- Use clear, descriptive filenames
- Organize with categories
- Use excerpt separator for homepage previews

## Technical Details

- Built with Jekyll 4.3
- Markdown processor: Kramdown
- Syntax highlighter: Rouge
- RSS feed included
- Mobile responsive
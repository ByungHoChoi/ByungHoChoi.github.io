---
title: "Learning Jekyll"
categories: learning
---

# Jekyll Blog Quick Guide
## 1. Important Files
`_config.yml`
Main site settings: title, URL, theme, author, plugins.
`/000.md`
Top-level pages (= categories). These become URLs like /papers/, /learning/, /life/.
`_posts/`
Actual blog posts live here.
`_site/`
Generated output. **Do not edit this.**
## 2. Writing A New Post
1. Create a file in _posts/:
_posts/YYYY-MM-DD-title.md
> Example:
> _posts/2026-06-30-my-first-paper-review.md

Post example:
```markdown
---
title: "My First Paper Review"
categories: papers
tags:
  - llm
  - systems
  - gpu
---
Write your post here.
```

## 3. Common Post Metadata
Put metadata in the front matter at the top of the post:
```
---
title: "Post Title"
categories: papers
tags:
  - tag1
  - tag2
---
```
### Useful fields:

```
title: "Post Title"
```
Post title.
```
categories: papers
```
Main category.
```
tags:
  - llm
  - gpu
  - systems
```
Tags are more detailed labels.
```
excerpt: "Short summary of the post."
```
Short description shown in lists/search.
```
date: 2026-06-30
```
Optional explicit date. Usually filename date is enough.
```
last_modified_at: 2026-06-30
```
Useful when updating old posts.
```
toc: true
```
Shows a table of contents for headings.
```
author_profile: true
```
Shows your profile sidebar.
```
published: false
```
Keeps the post from being published.

## 6. Local Preview
If you want to preview locally:
`bundle exec jekyll serve`
Open:
http://127.0.0.1:4000/

## 7. Publish

If you just want to publish:
```sh
git add .
git commit -m "Add new post"
git push
```
GitHub Actions builds and deploys the site automatically.

## 8. Rule Of Thumb

Edit these:
```
_posts/*.md
*.md
_config.yml
_data/navigation.yml
_includes/
assets/css/main.scss
```
Do not edit:
```
_site/
```
# Kevin Raymond GitHub Pages Blog Starter

This is a basic Jekyll-powered blog starter for GitHub Pages.

## What it includes

- Home page
- About page
- Archive page
- Sample blog post
- Simple custom styling
- Markdown post workflow

## How to use it

1. Create a new GitHub repository.
   - Easiest option for a personal site later: `yourusername.github.io`
   - Or use any repo name for now.
2. Upload all of these files to the repo.
3. If your repo is **not** named `yourusername.github.io`, edit `_config.yml` and set `baseurl` to `"/your-repository-name"`.
4. In GitHub, go to **Settings → Pages**.
5. Under **Build and deployment**, choose:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
6. Save.
7. Wait for GitHub Pages to publish the site.

If you use a normal repo name, your site URL will look like this:

`https://yourusername.github.io/repository-name/`

If you use `yourusername.github.io`, the site URL will be:

`https://yourusername.github.io/`

## Adding a new post

Create a file inside `_posts/` using this format:

`YYYY-MM-DD-your-post-title.md`

Example:

`2026-04-01-what-the-numbers-on-sheet-metal-mean.md`

Use this front matter at the top:

```yaml
---
title: Your Post Title
description: One sentence that explains what the post is about.
categories: [sheet-metal]
---
```

Then write the rest in Markdown.

## Editing pages

- `index.html` = home page settings
- `about.md` = about page
- `archive.md` = all posts page
- `assets/css/style.css` = site styling

## Images

Put images in:

`assets/images/`

Then insert them in a post like this:

```md
![Description]({{ '/assets/images/your-image.jpg' | relative_url }})
```

## When you move your domain later

Once you're ready to use `kevinraymond.me`, you can connect the domain in **Settings → Pages** and then update your DNS records at your domain registrar.

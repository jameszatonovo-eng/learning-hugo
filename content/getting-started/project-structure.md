---
title: "Project Structure"
description: ""
weight: ""
categories: []
tags: []
layout: ""
---


Hugo projects follow a predictable layout. Instead of configuring where everything “lives,” you place files into a few well-known directories and Hugo wires them together when it builds your site.

From a content author’s perspective, the most important idea is this: **your folder structure under `content/` becomes your site structure**. That makes URLs, sections, and navigation much easier to reason about.

## The directories you’ll see most often

### `content/`
This is where you write your site’s pages in Markdown. Hugo treats folders inside `content/` as **sections**, and files inside those folders as **pages**.

For example:

- `content/getting-started/project-structure.md` typically becomes `/getting-started/project-structure/`
- `content/concepts/_index.md` typically becomes the landing page for `/concepts/`

Because Hugo derives so much from the content tree, you can usually organize a site by simply creating folders and Markdown files—without extra routing configuration.

### `layouts/`
Layouts are HTML templates that control how content is rendered. When you view a page, Hugo selects a template based on things like:

- the page’s section/content type
- whether the page is a single page vs. a list page
- front matter parameters like `layout`

If you’re primarily authoring content, you may not touch `layouts/` often—but it’s useful to know that content and templates are kept separate.

### `static/`
Static files are copied directly into the final site without being processed. Typical examples include:

- images
- downloadable PDFs
- robots.txt or other files that should be served “as-is”

### `themes/`
Themes provide prebuilt templates, styles, and sometimes example content. A theme can dramatically change how your site looks and behaves without requiring you to rewrite your Markdown.

Many sites start with a theme and later override parts of it by adding templates to `layouts/`.

### `config/`
Configuration controls global settings such as:

- site title and base URL
- enabled languages
- taxonomy definitions (tags/categories)
- theme parameters

Hugo supports multiple configuration formats, but conceptually this folder is where you define site-wide behavior.

## Why Hugo’s structure works well

Hugo is intentionally opinionated. By standardizing where content, templates, assets, and configuration belong, it reduces the number of decisions you have to make before you can publish.

That predictability is especially valuable on teams: content authors can focus on writing in `content/`, and developers/designers can adjust presentation in `layouts/` or a theme.

## Key takeaways

- **`content/` is the center of the site**: it drives sections, URLs, and most page organization.
- **Folders map to site structure**: your information architecture is reflected directly in the file tree.
- **Hugo reduces configuration overhead** by using conventions for templates, static files, and settings.
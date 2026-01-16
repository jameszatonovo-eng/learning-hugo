---
title: "Pages Vs Sections"
description: ""
weight: ""
categories: []
tags: []
layout: ""
---

In Hugo, the structure of your site is primarily driven by the `content/` directory. Understanding the difference between **pages** and **sections** is essential because it affects URLs, navigation, and which templates Hugo chooses.

## Sections: folders under `content/`

A **section** is typically a top-level folder inside `content/`. For example:

- `content/getting-started/` defines the `getting-started` section
- `content/concepts/` defines the `concepts` section

Sections act like containers for related pages. Many themes render a section as a “list page” that shows links to the pages inside it.

## Pages: the individual content files

A **page** is usually a Markdown file that represents a single piece of content, such as:

- an article
- a documentation page
- an about page

For example, `content/concepts/front-matter.md` is a page.

## Section landing pages with `_index.md`

Hugo uses `_index.md` to create a **section landing page** (a page for the folder itself). This is how you add intro text, metadata, or custom layout behavior to a section.

For example:

- `content/concepts/_index.md` becomes the landing page for `/concepts/`

Without `_index.md`, a section can still exist, but you lose a clear place to store section-level content and settings.

## Bundles (high level)

Hugo also supports organizing content into **bundles**, which group a page with its resources (like images) in the same folder.

- **Branch bundles** are section-like and use `_index.md`.
- **Leaf bundles** are page-like and use `index.md`.

You don’t need to master bundles immediately, but it’s useful to know they exist when you start attaching images or other files to specific pages.

## Key takeaways

- **Sections** come from folders under `content/` and often render as list pages.
- **Pages** are individual Markdown files that render as single pages.
- `_index.md` creates a section landing page and is key for controlling hierarchy, metadata, and URLs.
---
title: "Front Matter"
description: ""
weight: ""
categories: []
tags: []
layout: ""
---

Front matter is the block of metadata at the top of a Hugo content file. It provides information *about* the content—things Hugo and your theme use to decide how the page should behave.

Think of front matter as the contract between your Markdown and the rest of the site: templates, navigation, sorting, and visibility often depend on it.

## What front matter controls

Common front matter fields include:

- `title`: the page title shown in headings and lists
- `date`: used for sorting and for “published on” metadata
- `draft`: marks content as unfinished so it can be hidden from production builds
- `weight`: a numeric value that controls ordering in menus and section lists
- `description`: used for summaries, list previews, and SEO metadata

Themes may also support additional fields such as `tags`, `categories`, `layout`, or custom parameters.

## Why it matters

In Hugo, content isn’t just text—it’s content *plus metadata*. Two pages with identical Markdown can render very differently depending on front matter:

- ordering in a section may change based on `date` or `weight`
- pages can be hidden if marked as `draft`
- templates can switch based on content type, section, or `layout`

## Supported formats (briefly)

Hugo supports multiple front matter formats (commonly YAML, TOML, and JSON). The important point is not the syntax, but that the metadata is machine-readable and consistent.

## Key takeaways

- Front matter is the metadata block that drives how Hugo and themes treat a page.
- Fields like `title`, `draft`, `date`, and `weight` influence ordering, visibility, and rendering.
- Treat front matter as the “control plane” for content behavior across your site.
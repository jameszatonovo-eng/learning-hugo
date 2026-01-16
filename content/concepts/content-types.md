---
title: "Content Types"
description: ""
weight: ""
categories: []
tags: []
layout: ""
---

In Hugo, a **content type** is a way to group content that should share similar templates and behavior. It’s an organizational concept, but it also has practical impact: Hugo uses content type to help decide which layouts to apply.

## How content type is determined

By default, Hugo infers content type from the directory structure under `content/`. In many projects:

- `content/blog/...` is treated as “blog” content
- `content/docs/...` (or `content/concepts/...`) is treated as “docs” style content

This convention means you often don’t need to set a content type manually—your folder structure becomes the signal.

## Why content types matter

Different content types often need different presentation:

- blog posts might show author, date, reading time, and tags
- documentation pages might prioritize a table of contents, section navigation, and ordering by `weight`

By separating content into types, Hugo can apply different templates and defaults without extra glue code.

## Example: blog vs documentation

If you keep posts in `content/blog/` and documentation in `content/getting-started/` or `content/concepts/`, you can configure your theme/layouts so that:

- blog lists are grouped/sorted by date
- docs lists are ordered by weight and show next/previous navigation

The content stays clean, while layout choices remain predictable.

## Key takeaways

- Content type helps Hugo choose appropriate layouts and behaviors.
- Hugo typically infers type from `content/` folder structure, reducing configuration.
- Separating content by type makes sites easier to maintain and scale as they grow.
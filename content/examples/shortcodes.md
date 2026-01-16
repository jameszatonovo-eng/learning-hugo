---
title: "Shortcodes"
description: ""
weight: ""
categories: []
tags: []
layout: ""
---

Shortcodes are Hugo’s way to embed reusable components inside Markdown content. They let you go beyond “plain Markdown” without forcing authors to write raw HTML.

You can think of a shortcode as a small, named snippet that expands into HTML (or another output) during the build.

## Why shortcodes are useful

Markdown is intentionally minimal. That’s great for writing, but real sites often need richer content such as:

- embedded videos
- images with captions
- callout boxes
- responsive layouts
- diagrams, charts, or custom UI elements

Shortcodes provide those features while keeping your content files readable and consistent.

## Content stays clean, templates stay powerful

Instead of sprinkling custom HTML everywhere, you can centralize complex markup in one shortcode implementation. Authors then use a simple shortcode call in Markdown.

This separation has practical benefits:

- content is easier to write and review
- design changes happen in one place (the shortcode), not across dozens of pages
- sites remain more consistent as they grow

## When to use shortcodes vs raw HTML

Shortcodes are a good fit when:

- you need the same “component” on multiple pages
- you want consistent styling/behavior
- you want to protect authors from fragile HTML

Raw HTML can still be useful for one-off cases, but it’s harder to maintain at scale.

## Key takeaways

- Shortcodes are reusable building blocks that extend Markdown inside Hugo.
- They keep content readable while still enabling complex layouts and embeds.
- Prefer shortcodes over repeated raw HTML when you want consistency and maintainability.
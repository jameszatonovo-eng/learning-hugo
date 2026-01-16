---
title: "Markdown"
description: ""
weight: ""
categories: []
tags: []
layout: ""
---

Markdown is the primary authoring format used by Hugo. It’s a lightweight markup language designed to be easy to write, easy to read in raw form, and simple to convert into HTML.

For content-heavy sites—documentation, blogs, course notes—Markdown is a great fit because it keeps the focus on writing, not on hand-crafting web markup.

## Why Hugo uses Markdown

Markdown gives Hugo a clean separation between:

- **content** (your words)
- **presentation** (the theme and templates)

Authors can write in plain text, while the site’s look and behavior stays controlled by layouts.

## Readable in Git, friendly for reviews

Because Markdown is text-based, it works well with version control. It’s easy to diff, review, and edit collaboratively. That makes it practical for teams and for long-lived sites.

## How Hugo extends Markdown

Hugo adds a few important ideas on top of basic Markdown:

- **Front matter**: metadata at the top of the file (title, draft status, ordering, etc.).
- **Shortcodes**: reusable components you can embed inside Markdown for richer content.

These extensions keep Markdown simple for writing while still supporting real-world publishing needs.

## Key takeaways

- Markdown is Hugo’s default content format because it’s simple, readable, and portable.
- Hugo’s themes and templates handle presentation so authors can focus on writing.
- Front matter and shortcodes extend Markdown to support metadata-driven behavior and richer page features.
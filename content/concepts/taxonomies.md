---
title: "Taxonomies"
description: ""
weight: ""
categories: []
tags: []
layout: ""
---

Taxonomies are Hugo’s built-in way to classify and group content. They help you answer questions like:

- “Show me all posts tagged `hugo`.”
- “List everything in the `tutorials` category.”

In practice, taxonomies make content easier to browse and improve navigation without forcing you to manually create index pages.

## What is a taxonomy?

A **taxonomy** is a named classification system. Hugo ships with two common ones by default:

- `tags`
- `categories`

Each taxonomy contains **terms** (the values you assign to content). For example, `tags` might contain terms like `hugo`, `markdown`, and `static-sites`.

## Declaring taxonomies in configuration

Taxonomies are declared at the site level in your configuration (for example, in `config/`). Conceptually, you’re telling Hugo:

- which taxonomies exist
- what their URL paths should look like

Once declared, Hugo knows how to organize content around those taxonomies.

## Applying taxonomies in front matter

You attach taxonomies to pages through front matter. For instance, adding values to `tags` or `categories` associates that page with the corresponding taxonomy terms.

The result is that a single piece of content can belong to multiple groups at once (for example, a page can have several tags).

## Automatic listing pages

One of the benefits of Hugo taxonomies is that Hugo can generate listing pages automatically:

- a page that lists all terms (for example, all tags)
- a page per term (for example, everything tagged `hugo`)

Even without writing custom templates, a theme will often provide reasonable defaults for these pages.

## Key takeaways

- Taxonomies are Hugo’s mechanism for organizing content by **shared labels** like tags and categories.
- You define taxonomies in site configuration and apply them via **front matter**.
- Hugo can generate taxonomy listing pages automatically, which improves discoverability and navigation.
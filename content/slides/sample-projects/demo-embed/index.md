---
title: "Demo: Markdown with Embedded HTML"
date: 2026-08-25
categories: ["Sample Projects"]
access: public
---

## Introduction

This is a sample page demonstrating how to write **Markdown content** and embed interactive HTML pages from the `static/` folder at the same time.

You can write normal Markdown here — headings, lists, code blocks, links, images — anything you like.

## Embedded Slide: If Conditions

Below is an interactive slide about "If Conditions" embedded directly into this Markdown page:

{{< embed-html src="/slides-html/coding-basics/if/index.html" height="600px" >}}

## Some More Markdown Content

As you can see, the embedded HTML page appears inline with the rest of the content. You can continue writing after it.

### Key Takeaways

- You can mix Markdown text with embedded HTML pages freely
- The `embed-html` shortcode supports customizing `height`, `width`, and toggling the fullscreen button
- Each embedded page has its own fullscreen button for a better viewing experience

## Another Embedded Slide: Switch Statement

Here's another example with a different slide:

{{< embed-html src="/slides-html/coding-basics/switch/index.html" height="500px" >}}

## Shortcode Parameters

| Parameter    | Default  | Description                          |
|-------------|----------|--------------------------------------|
| `src`       | (required) | Path to HTML file in `static/`     |
| `height`    | `600px`  | Height of the iframe                 |
| `width`     | `100%`   | Width of the container               |
| `fullscreen`| `true`   | Show fullscreen button (`true`/`false`) |

## Example Without Fullscreen Button

{{< embed-html src="/slides-html/coding-basics/oop/index.html" height="400px" fullscreen="false" >}}

---

That's it! This page shows how Markdown and embedded HTML can coexist seamlessly.

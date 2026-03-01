# Your GitHub Learning Lab Repository for Introducing GitHub

Welcome to **your** repository for your GitHub Learning Lab course. This repository will be used during the different activities that I will be guiding you through. See a word you don't understand? We've included an emoji 📖 next to some key terms. Click on it to see its definition.

Oh! I haven't introduced myself...

I'm the GitHub Learning Lab bot and I'm here to help guide you in your journey to learn and master the various topics covered in this course. I will be using Issue and Pull Request comments to communicate with you. In fact, I already added an issue for you to check out.

![issue tab](https://lab.github.com/public/images/issue_tab.png)

I'll meet you over there, can't wait to get started!

This course is using the :sparkles: open source project [reveal.js](https://github.com/hakimel/reveal.js/). In some cases we’ve made changes to the history so it would behave during class, so head to the original project repo to learn more about the cool people behind this project.

---

## What is this repository?

This repository is an **interactive slideshow presentation** built with [Jekyll](https://jekyllrb.com/) and [reveal.js](https://github.com/hakimel/reveal.js/). It serves as a hands-on learning environment for the *Introducing GitHub* course on GitHub Learning Lab.

### How it works

- **Jekyll** (a static site generator) processes the repository and builds a website from the source files.
- **reveal.js** renders that website as a beautiful, browser-based slide deck with keyboard/touch navigation, transitions, and more.
- Each slide is a **Markdown file** stored in the `_posts/` directory. Jekyll collects all posts and renders them as individual slides in chronological order.
- The overall slide layout and reveal.js configuration live in `_layouts/` and `_config.yml`.

### Key files and directories

| Path | Purpose |
|------|---------|
| `_posts/` | Individual slide content (Markdown) |
| `_layouts/` | HTML templates for slides and the full presentation |
| `_includes/` | Reusable HTML partials (e.g. a single slide wrapper) |
| `_config.yml` | Jekyll & reveal.js configuration (theme, transitions, slide size, …) |
| `index.html` | Entry point — iterates over posts and assembles the slide deck |
| `Gemfile` | Ruby gem dependencies (Jekyll, plugins) |
| `package.json` | Node.js dependencies (reveal.js) |
| `script/` | Helper scripts for the Learning Lab course |

### Adding a new slide

Create a new Markdown file in `_posts/` following the naming convention `YYYY-MM-DD-title.md` and include the front-matter:

```markdown
---
layout: slide
title: "My new slide"
---

Slide content goes here.
```

Jekyll will automatically pick it up and insert it into the presentation.

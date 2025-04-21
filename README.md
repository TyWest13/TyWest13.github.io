# The Tactile theme

[![Build Status](https://travis-ci.org/pages-themes/jekyll-theme-tactile.svg?branch=master)](https://travis-ci.org/pages-themes/jekyll-theme-tactile) [![Gem Version](https://badge.fury.io/rb/jekyll-theme-tactile.svg)](https://badge.fury.io/rb/jekyll-theme-tactile)

*Tactile is a Jekyll theme for GitHub Pages. You can [preview the theme to see what it looks like](http://pages-themes.github.io/tactile), or even [use it today](#usage).*

## Usage

To use the Tactile theme:

1. Add the following to your site's `_config.yml`:

```yml
theme: jekyll-theme-tactile
title: Custom title
description: Custom description.
show_downloads: true
google_analytics:
```

- To override the repository name or description from GitHub used in the header, set a `title` or `description`.
- Set `show_downloads` to `false` to hide the download buttons in the header.
- Set `google_analytics` to your tracking ID to enable pageview tracking.

This theme includes a single `default` layout. Markdown files should be prefixed with the following frontmatter.

```
---
layout: default
---

```

#### CSS

For CSS customization, create your own `/assets/css/styles.scss` in your project to replace the one from this theme, and override selected stylesheet properties.

```scss
---
---
@import "rouge-base16-dark";
@import "tactile";
```

#### Syntax Highlighting

[Rouge](http://rouge.jneen.net/) is the default highlighter in Jekyll 3. This theme includes the `base16.dark` stylesheet from Rouge.

To switch syntax highlighting colors to say `monokai`, install the `rouge` gem and run the following on the command line.

```
mkdir _scss
rougify style monokai > _scss/rouge-monokai.scss
```

Then replace `rouge-base16-dark` with `rouge-monokai` in `/assets/css/styles.scss`

Other pygments highlighter themes should work as well.

# Sprocket
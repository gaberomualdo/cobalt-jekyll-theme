# Cobalt

*Cobalt a minimalistic, simple Jekyll theme for a blog and personal website.*.

[Theme preview](https://xtrp.github.io/cobalt-jekyll-theme/)

![Cobalt theme preview](/screenshot.png)

## Installation

Download this Github repository.

### Layouts

Refers to files within the `_layouts` directory, that define the markup for your theme.

  - `default.html` &mdash; The base layout that lays the foundation for subsequent layouts. The derived layouts inject their contents into this file at the line that says ` {{ content }} ` and are linked to this file via [FrontMatter](https://jekyllrb.com/docs/frontmatter/) declaration `layout: default`.
  - `home.html` &mdash; The layout for your landing-page / home-page / index-page. [[More Info.](#home-layout)]
  - `page.html` &mdash; The layout for your documents that contain FrontMatter, but are not posts.
  - `post.html` &mdash; The layout for your posts.

### Includes

Refers to snippets of code within the `_includes` directory that can be inserted in multiple layouts (and another include-file as well) within the same theme-gem.

  - `footer.html` &mdash; Defines the site's footer section.
  - `google-analytics.html` &mdash; Inserts Google Analytics module.
  - `head.html` &mdash; Code-block that defines the `<head></head>` in *default* layout.
  - `header.html` &mdash; Defines the site's main header section.
  - `nav.html` &mdash; Defines the post layouts top bar.

### Assets

Refers to various asset files within the `assets` directory.
Contains the `main.css`, the theme's main stylesheet called by `_layouts/default.html` via `_includes/head.html`.

This directory can include sub-directories to manage assets of similar type, and will be copied over as is, to the final transformed site directory.

### Plugins

Cobalt comes with [`jekyll-seo-tag`](https://github.com/jekyll/jekyll-seo-tag) plugin preinstalled to make sure your website gets the most useful meta tags. See [usage](https://github.com/jekyll/jekyll-seo-tag#usage) to know how to set it up.

### Home Layout

`home.html` is a flexible HTML layout for the site's landing-page / home-page / index-page. <br/>

### Enabling Google Analytics

To enable Google Analytics, add the following lines to your Jekyll site:

```yaml
  google_analytics: UA-NNNNNNNN-N
```

### FrontMatter in Posts

Posts should have the following variables in their FrontMatter:

 - `layout` &mdash; defines the layout of the page, and should be defined as `post`
 - `read_time` &mdash; the amount of time the post should take to read, in minutes.
 - `author` &mdash; the author of the post.
 - `date` &mdash; the date the post was written and published.

## License

The theme is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

## Credits

Cobalt was developed by [Fred Adams](https://xtrp.github.io).

Cobalt is built on top of the default [Minima theme](https://jekyll.github.io/minima/), which was built by Parker Moore and the minima contributors.

The SVG icons used in the Cobalt theme can all be found on [iconmonstr](http://iconmonstr.com).

Cobalt uses [Skeleton.css](http://getskeleton.com), a responsive CSS boilerplate.

Cobalt also uses [normalize.css](https://necolas.github.io/normalize.css/), a modern alternative to CSS resets.

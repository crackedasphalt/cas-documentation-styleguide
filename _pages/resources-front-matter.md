---
title: "All YAML Front Matter"
toc: true
toc_sticky: true
excerpt: All YAML Front Matter Tags
hidden: false
permalink: /resources-front-matter/
header:
  image: /assets/images/home/home-page-feature.jpg
  overlay_image: /assets/images/home/home-page-feature.jpg
  teaser: /assets/images/home/home-page-feature.jpg
classes: no-sidebar
---

## All Page Types

### Informational
```yaml
title: # "string" - Assign a meaningful title to appear on page
layout: # archive-wide, archive, categories, catgories-wide, category, collection, home, posts, single, splash, tag-wide, tag, tags
excerpt: # Don't use description front matter, use this instead
excerpt_separator: "<!--more-->" # For long excerpts, place "<!--more-->" in page contents where excerpt should end.
tagline: # This is a custom tagline content which overrides the *default* page excerpt.
date: # 2022-05-27T11:59:26-08:00 - Published Date, overrides date in the file name of a post.
last_modified_at: # 2022-05-27T11:59:26-08:00 - Last Updated Date.
```

### Attribution
```yaml
author_profile: # false, true - Displays author profile on page left
author: # Author name - Overrides the default site author.
```

### Navigation
```yaml
permalink: # /multiple/dirs/possible/ - optional for posts with categories
canonical_url: # https://www.crackedasphalt.com/permalink/ - Places canonical url in page
redirect_from: # Use if pages have moved or to blackhole a page
  - /some/path/ # Relative path of redirecting page.
  - /another/path/file.pdf.html # If redirecting page has file extension, append with ".html"
```

### Table of Contents
```yaml
toc: # false, true. Displays table of contents.
toc_label: # "A Custom Label" Assigns unique title to table of contents, overrides toc_label from _data/ui-text.yml
toc_icon: # "heart" - Assigns "heart" corresponding Font Awesome icon name (use without font awesome prefix)
toc_sticky: # false, true - Makes table of contents sticky on page.
```

### Search and Find
```yaml
sitemap: # false, true - Excludes or includes page from /sitemap/ and sitemap.xml
hidden: # false, true - Excludes or includes page from displaying in archive views. Useful with posts. Use in junction with "search:"
search: # false, true - Excludes or includes page from being displayed in site search index. Only works with lunr search.
```

### Display and Hide Elements
```yaml
hide-signup-form: # false, true - Hides signup form in footer
header: # Enable header
  image: # /path/to/image.jpg - Full image displayed. Does not display if overlay_x is also defined. If defined, is used for Open Graph.
  overlay_image: # /path/to/overlay_image.jpg - Will prevent "image:" from displaying on page.
  overlay_color: # "#5e616c" - Color of header overlay mask
  overlay_filter: .5 # Accepts decimal number 0<x<1, RGBA for non-black "rgba(255, 0, 0, 0.5)", or linear-gradient(rgba(255, 0, 0, 0.5), rgba(0, 255, 255, 0.5))
  caption: # "Photo credit: [**Unsplash**](https://unsplash.com)" - Displays a caption 
  actions: # Defines an action link in header
    - label: # "<i class='fas fa-mountain-city'></i> Get started" - Text of action link.
      url: # "/some/path/" - Path to action link.
  teaser: # /path/to/image.jpg - Teasers appear on archive pages and related posts
  og_image: # Optional OpenGraph override image.
  show_overlay_excerpt: # true (default), false - Toggles display of page excerpt in page hero
```

### Galleries
To include gallery body of page must include some variation of below.  See [here][resources-gallery] for examples.

```{% raw %}{% include gallery caption="Caption" %}{% endraw %}```

```yaml
gallery:
  - url: # /assets/images/styleguide/unsplash-gallery-image-1.jpg - Path to full res image 1
    image_path: # /assets/images/styleguide/unsplash-gallery-image-1-th.jpg - Path to thumbnail for image 1
    alt: # "placeholder image 1" - Alt text for image 1
    title: # "Image 1 title caption" - Display title for image 1
  - url: # /assets/images/styleguide/unsplash-gallery-image-2.jpg - Path to full res image 2, 3, 4, etc.
    image_path: # /assets/images/styleguide/unsplash-gallery-image-2-th.jpg - Path to thumbnail for image 2, 3, 4, etc.
    alt: # "placeholder image 2" - Alt text for image 2, 3, 4, etc.
    title: # "Image 2 title caption" - Display title for image 2, 3, 4, etc.
path_gallery:
  path: # "/assets/images/home" - Path to the directory containing images
  exts: 
   - jpg # Some image file extension
   - png # Another image file extension
```

### Feature Row
To include feature row, body of page must include the below. See [here][resources-includes] for examples.

```{% raw %}{% include feature_row %}{% endraw %}```

```yaml
feature_row: # Include liquid tag: "% include feature_row %"
  - image_path: /assets/images/home/feature-one.jpg
    image_caption: # Optional "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Current projects"
    title: "Current projects"
    excerpt: "Some language here about current projects that are ongoing.<br />"
    url: "/feature-one/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/home/feature-two.jpg
    image_caption: # Optional "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Build gallery"
    title: "Build gallery"
    excerpt: "A collection of finished products. This should be a list of gallery links."
    url: "/feature-two/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/home/feature-three.jpg
    image_caption: # Optional "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Make it yourself"
    title: "Make it yourself"
    excerpt: "Some information about myog. Link to page containing guides."
    url: "/feature-three/"
    btn_class: "btn--primary"
    btn_label: "Get yours"
```

### Intro
To include an intro, body of page must include the below. See [here][resources-includes] for examples.

```{% raw %}{% include feature_row id="intro" type="center" %}{% endraw %}```

```yaml
intro: # Displayed below header image or header overlay image
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'
```

### Formatting and Layout Adjustments

```yaml
classes: 
 - # wide - Widens the main content of the page to the right
 - # no-sidebar eliminates left side bar
sidebar: # Custom left sidebar options.
  - title: # "Title" - Some title
    image: # http://place-hold.it/350x250 - an image related to title
    image_alt: # "image" - alt
    text: # "Some text here."
  - title: # "Another Title" - Some title
    text: # "More text here."
  - title: # "Sample Title"
    nav: # "sidebar-sample" references the sidebar-sample key in _data/navigation.yml so make sure they match.
```

## Posts

```yaml
categories: 
  - Jekyll
  - Another
tags:
  - content
  - excerpt
  - layout
  - pinned
link: https://github.com # To turn a post in to a link post
show_date: # true, false - disables date display in posts, 
comments: # true, false - turns comments on and off in posts.
read_time: # true, false
related: # true, false
share: # true, false
```

## Archive Pages

{% capture fm01 %}show_pinned: true # Displays posts with tag "pinned" at front of list
show_teasers: true # Always display teasers{% endcapture %}
```yaml
{{fm01}}
```

## Category Pages

{% capture fm02 %}entries_layout: # list (default), grid - Use on layouts category, tag, category-wide, tag-wide
taxonomy: Layout # category, tag, category-wide, tag-wide / category name{% endcapture %}
```yaml
{{fm01}}
{{fm02}}
```

## Tag Pages

```yaml
{{fm01}}
{{fm02}}
```

## Collection Pages

```yaml
collection: # "collectionname" - Collection name. Collection must be defined in _config.yml
entries_layout: # list (default), grid -  - Use on layouts category, tag, category-wide, tag-wide
```


[resources-includes]: {{ "" | relative_url }}{% link _pages/resources-includes.md %}
[resources-gallery]: {{ "" | relative_url }}{% link _pages/resources-gallery.md %}

---
title: "Includes Examples"
excerpt: A variety of common includes and their YAML Front Matter.
classes: no-sidebar
toc: true
toc_sticky: true
feature_row:
  - image_path: /assets/images/styleguide/mm-customizable-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Home page feature"
    title: "Home Page Feature"
    excerpt: "Some language about home pages."
    url: "/feature-one/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/styleguide/mm-free-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Free"
    title: "Free"
    excerpt: "Some language about being free.<br /><br />"
    url: "/feature-two/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/styleguide/mm-responsive-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Responsive"
    title: "Responsive"
    excerpt: "Some information about being responsive."
    url: "/feature-three/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
feature_row2:
  - image_path: /assets/images/styleguide/mm-customizable-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row3:
  - image_path: /assets/images/styleguide/mm-customizable-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/images/styleguide/mm-customizable-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
intro: # Displayed below header image or header overlay image
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'
---

## Gallery
For gallery examples, see the gallery resources page [here][resources-gallery].

## Feature Row

### Three Features

Use this front matter

```yaml
feature_row:
  - image_path: /assets/images/styleguide/mm-customizable-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Home page feature"
    title: "Home Page Feature"
    excerpt: "Some language about home pages."
    url: "/feature-one/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/styleguide/mm-free-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Free"
    title: "Free"
    excerpt: "Some language about being free."
    url: "/feature-two/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/styleguide/mm-responsive-feature.png
    image_caption: Optional "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Responsive"
    title: "Responsive"
    excerpt: "Some information about being responsive."
    url: "/feature-three/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
```

Place the feature row using below

```liquid
{% raw %}{% include feature_row %}{% endraw %}
```

Example:

{% include feature_row %}

### One Feature/Left Align

Use this front matter

```yaml
feature_row2:
  - image_path: /assets/images/styleguide/mm-customizable-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
```

Place the feature row using below

```liquid
{% raw %}{% include feature_row id="feature_row2" type="left" %}{% endraw %}
```

Example:

{% include feature_row id="feature_row2" type="left" %}

### One Feature/Right Align

Use this front matter

```yaml
feature_row3:
  - image_path: /assets/images/styleguide/mm-customizable-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
```

Place the feature row using below

```liquid
{% raw %}{% include feature_row id="feature_row3" type="right" %}{% endraw %}
```

Example:

{% include feature_row id="feature_row3" type="right" %}

### One Feature Center Align

Use this front matter

```yaml
feature_row4:
  - image_path: /assets/images/styleguide/mm-customizable-feature.png
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
```

Place the feature row using below

```liquid
{% raw %}{% include feature_row id="feature_row4" type="center" %}{% endraw %}
```

Example:

{% include feature_row id="feature_row4" type="center" %}


## Intro

Use this front matter

```yaml
intro: # Displayed below header image or header overlay image
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'
```
Place the intro using the below

```liquid
{% raw %}{% include feature_row id="intro" type="center" %}{% endraw %}
```

Example:

{% include feature_row id="intro" type="center" %}

[resources-gallery]: {{ "" | relative_url }}{% link _styleguide/resources-gallery.md %}
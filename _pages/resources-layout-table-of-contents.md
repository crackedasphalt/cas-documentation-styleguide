---
title: "Layout: Table of Contents"
permalink: /resources-layout-table-of-contents/
toc: true
excerpt: A page with table of contents.
---

Enable table of contents on post or page by adding `toc: true` to its YAML Front Matter. The title and icon can also be changed with:

```yaml
---
toc: true
toc_label: "Unique Title"
toc_icon: "heart"  # corresponding Font Awesome icon name (without fa prefix)
toc_sticky: # false (default), true
---
```

Alternatively, add helper code

```
{% raw %}{% include toc %}{% endraw %}
```
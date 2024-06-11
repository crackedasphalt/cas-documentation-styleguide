---
title: "Embedded Content"
toc: true
excerpt: Examples of embedded content. 
permalink: /resources-embedded-content/
---

## Image

The preferred way of using images is placing them in the `/assets/images/` directory and referencing them with an absolute path. Prepending the filename with `{% raw %}{{ site.url }}{{ site.baseurl }}/assets/images/{% endraw %}` will make sure your images display properly in feeds and such.

**Absolute path:**

![Absolute]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/unsplash-gallery-image-3.jpg)

```markdown
{% raw %}![Absolute]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/unsplash-gallery-image-3.jpg){% endraw %}
```

**Relative path:**

![Relative]({{ '/assets/images/styleguide/unsplash-gallery-image-3.jpg' | relative_url }})

```markdown
{% raw %}![Relative]({{ '/assets/images/styleguide/unsplash-gallery-image-3.jpg' | relative_url }}){% endraw %}
```

### Standard image with no width modifier classes applied.

**HTML:**

```html
{% raw %}<img src="{{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg" alt="">{% endraw %}
```

**or Kramdown:**

```markdown
{% raw %}![alt]({{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg){% endraw %}
```


### Image that fills page content container

Add the `.full` class with as below

**HTML:**

```html
{% raw %}<img src="{{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg" alt="" class="full">{% endraw %}
```

**or Kramdown:**

```markdown
{% raw %}![alt]({{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg)
{: .full}{% endraw %}
```

### Image with Link

[![foo](https://live.staticflickr.com/8361/8400335147_5fabaa504c_o.jpg)](https://flic.kr/p/dNiUYB)

```markdown
[![foo](https://live.staticflickr.com/8361/8400335147_5fabaa504c_o.jpg)](https://flic.kr/p/dNiUYB)
```

### Image with Caption

{% capture fig_img %}
![Foo]({{ '/assets/images/styleguide/unsplash-gallery-image-3.jpg' | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo from Unsplash.</figcaption>
</figure>

```markdown
{% raw %}{% capture fig_img %}
![Foo]({{ '/assets/images/styleguide/unsplash-gallery-image-3.jpg' | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo from Unsplash.</figcaption>
</figure>{% endraw %}
```

### Image Linked with Caption

{% capture fig_img %}
[![Foo](https://images.unsplash.com/photo-1541943869728-4bd4f450c8f5?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=800&fit=max&ixid=eyJhcHBfaWQiOjF9)](https://unsplash.com/)
{% endcapture %}

{% capture fig_caption %}
Stairs? Were we're going we don't need no stairs.
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>{{ fig_caption | markdownify | remove: "<p>" | remove: "</p>" }}</figcaption>
</figure>

```markdown
{% raw %}{% capture fig_img %}
[![Foo](https://images.unsplash.com/photo-1541943869728-4bd4f450c8f5?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=800&fit=max&ixid=eyJhcHBfaWQiOjF9)](https://unsplash.com/)
{% endcapture %}

{% capture fig_caption %}
Stairs? Were we're going we don't need no stairs.
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>{{ fig_caption | markdownify | remove: "<p>" | remove: "</p>" }}</figcaption>
</figure>{% endraw %}
```

## YouTube Video

**HTML:**
Creates embedded YouTube video.

<iframe width="640" height="360" src="https://www.youtube-nocookie.com/embed/-PVofD2A9t8?controls=0" frameborder="0" allowfullscreen></iframe>
<br />

```html
<iframe width="640" height="360" src="https://www.youtube-nocookie.com/embed/-PVofD2A9t8?controls=0" frameborder="0" allowfullscreen></iframe>
```

**Liquid:**

To embed the following YouTube video at url `https://www.youtube.com/watch?v=-PVofD2A9t8` (long version) or `https://youtu.be/-PVofD2A9t8` (short version) into a post or page's main content you'd use: 

```liquid
{% raw %}{% include video id="-PVofD2A9t8" provider="youtube" %}{% endraw %}
```

{% include video id="-PVofD2A9t8" provider="youtube" %}

**YAML Front Matter in Header:**

To embed it as a video header you'd use the following YAML Front Matter

```yaml
header:
  video:
    id: -PVofD2A9t8
    provider: youtube
```

## Vimeo

**Liquid:**

To embed the following Vimeo video at url `https://vimeo.com/212731897` into a post or page's main content you'd use: 

```liquid
{% raw %}{% include video id="212731897" provider="vimeo" %}{% endraw %}
```

{% include video id="212731897" provider="vimeo" %}

**YAML Front Matter in Header:**

To embed it as a video header you'd use the following YAML Front Matter

```yaml
header:
  video:
    id: 212731897
    provider: vimeo
```

## Twitter

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">🎨 Finally got around to adding all my <a href="https://twitter.com/procreateapp">@procreateapp</a> creations with time lapse videos <a href="https://t.co/1nNbkefC3L">https://t.co/1nNbkefC3L</a> <a href="https://t.co/gcNLJoJ0Gn">pic.twitter.com/gcNLJoJ0Gn</a></p>&mdash; Michael Rose (@mmistakes) <a href="https://twitter.com/mmistakes/status/662678050795094016">November 6, 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

```html
<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">🎨 Finally got around to adding all my <a href="https://twitter.com/procreateapp">@procreateapp</a> creations with time lapse videos <a href="https://t.co/1nNbkefC3L">https://t.co/1nNbkefC3L</a> <a href="https://t.co/gcNLJoJ0Gn">pic.twitter.com/gcNLJoJ0Gn</a></p>&mdash; Michael Rose (@mmistakes) <a href="https://twitter.com/mmistakes/status/662678050795094016">November 6, 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
```

## PDF

**HTML:**
Creates embedded PDF document.

<embed src="{{site.url}}/{{site.baseurl}}/assets/images/styleguide/crackedasphalt.com-Cracked-Asphalt.pdf#toolbar=0&navpanes=0&scrollbar=0" type="application/pdf">

Use this html tag
```html
<embed src="/assets/images/styleguide/crackedasphalt.com-Cracked-Asphalt.pdf#toolbar=0&navpanes=0&scrollbar=0" type="application/pdf">
```

**Liquid:**

To embed a PDF document at path `/assets/images/styleguide/crackedasphalt.com-Cracked-Asphalt.pdf` into a post or page's main content you'd use: 

```liquid
{% raw %}{% include embedded_document id="/assets/images/styleguide/crackedasphalt.com-Cracked-Asphalt.pdf" type="pdf" %}{% endraw %}
```

{% include embedded_document id="/cas-documentation-styleguide/assets/images/styleguide/crackedasphalt.com-Cracked-Asphalt.pdf" type="pdf" %}

## Google Map

**HTML:**
Creates embedded Google Map.

<iframe src="https://www.google.com/maps/d/u/4/embed?mid=1y4qCHS9zeQ1ake3ZpILre0QkH_Acwg0&ehbc=2E312F" width="640" height="480" frameborder="0"></iframe>
<br />

```html
<iframe src="https://www.google.com/maps/d/u/4/embed?mid=1y4qCHS9zeQ1ake3ZpILre0QkH_Acwg0&ehbc=2E312F" width="640" height="480" frameborder="0"></iframe>
```

**Liquid:**

To embed the following Google Map url `https://www.google.com/maps/d/u/4/edit?mid=1y4qCHS9zeQ1ake3ZpILre0QkH_Acwg0&usp=sharing` (with sharing parameter) or `https://www.google.com/maps/d/u/4/edit?mid=1y4qCHS9zeQ1ake3ZpILre0QkH_Acwg0` (without sharing parameter) into a post or page's main content you'd use: 

```liquid
{% raw %}{% include map id="1y4qCHS9zeQ1ake3ZpILre0QkH_Acwg0" provider="google" %}{% endraw %}
```

{% include map id="1y4qCHS9zeQ1ake3ZpILre0QkH_Acwg0" provider="google" %}
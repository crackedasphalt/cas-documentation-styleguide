---
title: "Gallery Examples"
excerpt: A variety of common gallery configurations.
gallery:
  - url: /assets/images/styleguide/unsplash-gallery-image-1.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-2.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-3.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 3"
    title: "Image 3 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-1.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 4"
    title: "Image 4 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-2.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 5"
    title: "Image 5 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-3.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 6"
    title: "Image 6 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-1.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 7"
    title: "Image 7 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-2.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 8"
    title: "Image 8 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-3.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 9"
    title: "Image 9 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-1.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 10"
    title: "Image 10 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-2.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 11"
    title: "Image 11 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-3.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 12"
    title: "Image 12 title caption"
gallery2:
  - url: https://flic.kr/p/8a6Ven
    image_path: https://farm2.staticflickr.com/1272/4697500467_8294dac099_q.jpg
    alt: "Black and grays with a hint of green"
  - url: https://flic.kr/p/8a738X
    image_path: https://farm5.staticflickr.com/4029/4697523701_249e93ba23_q.jpg
    alt: "Made for open text placement"
  - url: https://flic.kr/p/8a6VXP
    image_path: https://farm5.staticflickr.com/4046/4697502929_72c612c636_q.jpg
    alt: "Fog in the trees"
gallery3:
  - image_path: /assets/images/styleguide/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
  - image_path: /assets/images/styleguide/unsplash-gallery-image-4-th.jpg
    alt: "placeholder image 4"
gallery4:
  - url: /assets/images/styleguide/unsplash-gallery-image-1.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "Image 1 title caption"
classes: no-sidebar
toc: true
---

These are gallery tests for image wrapped in `<figure>` elements.

In all cases, information about the image will be captured in the following ways

| Thing                      | YAML Element     | Path Gallery Equivalent | Description                    |
| ------                     | --------         | ----------------------- | ------------------------------ |
| Gallery identifier         | `gallery:`          | `path_gallery:`     | Main element. This is also the value of the `id=""`. For path galleries, `id="path_gallery"` |
| URL of image               | `url:`              | url of image  | This is the source of the full-res image you are referencing. |
| Path to image (thumbnail)  | `image_path:`       | url of image  | This is the thumbnail or image shown on the page. |
| Alt tag of image           | `alt:`              | file name  | A visible alt tag on mouseover. |
| Title of image when viewed | `title:`            | file name  | The title of the image is displayed when opened. |
| Gallery caption | `caption="something"`            | `caption="something"`   | Caption of the gallery. |

## Define a Gallery Using YAML Front Matter

### Basic

To place a gallery add the necessary YAML Front Matter:

```yaml
gallery:
  - url: /assets/images/styleguide/unsplash-gallery-image-1.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-2.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-3.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 3"
    title: "Image 3 title caption"
  - url: /assets/images/styleguide/unsplash-gallery-image-4.jpg
    image_path: /assets/images/styleguide/unsplash-gallery-image-4-th.jpg
    alt: "placeholder image 4"
    title: "Image 4 title caption"
```


And then drop-in the gallery include --- gallery `caption` is optional.

```liquid
{% raw %}{% include gallery caption="This is a sample gallery with **Markdown support**." %}{% endraw %}
```

{% include gallery caption="This is a sample gallery with **Markdown support**." %}

This is some text after the gallery just to make sure that everything aligns properly. This needs to be extra long because the front matter of this page defines that there is no left hand side bar which means more space for content.

### Using a Gallery ID

Here comes another gallery, this time set the `id` to match 2nd gallery hash in YAML Front Matter.

```yaml
gallery2: # This is the 'id'
  - url: https://flic.kr/p/8a6Ven
    image_path: https://farm2.staticflickr.com/1272/4697500467_8294dac099_q.jpg
    alt: "Black and grays with a hint of green"
  - url: https://flic.kr/p/8a738X
    image_path: https://farm5.staticflickr.com/4029/4697523701_249e93ba23_q.jpg
    alt: "Made for open text placement"
  - url: https://flic.kr/p/8a6VXP
    image_path: https://farm5.staticflickr.com/4046/4697502929_72c612c636_q.jpg
    alt: "Fog in the trees"
```

And place it like so: 

```liquid
{% raw %}{% include gallery id="gallery2" caption="This is a second gallery example with images hosted externally." %}{% endraw %}
```

{% include gallery id="gallery2" layout="third" caption="This is a second gallery example with images hosted externally." %}


## Define a Gallery Using Contents of Static Folder

We can also define a gallery as all images in a static folder. This will only work on folders that are within the Jekyll project and only in locations that are considered [static files](https://jekyllrb.com/docs/static-files/).

To do this, a few things need to be true.  First, YAML Front Matter must contain 

```yaml
path_gallery:
  path: "/assets/images/home" # Define the path where images are stored
  exts: # Extensions to include in this gallery, one per line
   - jpg
   - png
```


Second, an include statement that specifies that this is a path-based gallery must be inserted in to page.

**You must specify `id="path_gallery"`. Nothing else will trigger this.**

```liquid
{%raw%}{% include gallery id="path_gallery" caption="This is a gallery from a folder collection." %}{%endraw%}
```


## Styling

Various stylings exist to modify the layout of a galllery.

### Fill Page Content Container

To fill page content container add `class="full"`.

```liquid
{% raw %}{% include gallery id="gallery3" class="full" caption="This is a third gallery example with two images and fills the entire content container." %}{% endraw %}
```

{% include gallery id="gallery3" class="full" caption="This is a third gallery example with two images and fills the entire content container." %}

### Number of Columns in Gallery
Configure how many columns are in the gallery by setting a layout. Gallery column layout can be overrided by setting a `layout`.

Certain layouts happen automatically. Others must be specified. Use the below table.

| Default at | Gallery Layout Name | Gallery Layout Description | Manual Override |
|------------|---------------------|----------------------------|-----------------|
| 1 image | uno | Single image spanning whole width of page. | `layout="uno"` |
| 2 images | half | Two images side by side. | `layout="half"` |
| >=3 images | third | Three images across. |`layout="third"` |
| Never default. Must be called manually | quarter | Four images across. | `layout="quarter"` |

#### One

```liquid
{% raw %}{% include gallery id="gallery4" layout="uno" caption="This is an uno gallery layout example." %}{% endraw %}
```

{% include gallery id="gallery4" layout="uno" caption="This is an uno gallery layout example." %}

#### Two

```liquid
{% raw %}{% include gallery id="gallery" layout="half" caption="This is a half gallery layout example." %}{% endraw %}
```

{% include gallery id="gallery" layout="half" caption="This is a half gallery layout example." %}

#### Three

```liquid
{% raw %}{% include gallery id="gallery" layout="third" caption="This is a third gallery layout example." %}{% endraw %}
```

{% include gallery id="gallery" layout="third" caption="This is a half gallery layout example." %}

#### Four

```liquid
{% raw %}{% include gallery id="gallery" layout="quarter " caption="This is a quarter gallery layout example." %}{% endraw %}
```

{% include gallery id="gallery" layout="quarter" caption="This is a quarter gallery layout example." %}
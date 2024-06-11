---
title: "Common Markup"
permalink: /resources-markup/
toc: true
excerpt: A variety of common markup.
toc_icon: "heart"
tags:
  - pinned
---

A variety of common markup showing how the theme styles them.

# Header one

## Header two

### Header three

#### Header four

##### Header five

###### Header six

```markdown
# Header one

## Header two

### Header three

#### Header four

##### Header five

###### Header six
```

## Blockquotes

Single line blockquote:

> Stay hungry. Stay foolish.

```markdown
> Stay hungry. Stay foolish.
```

Multi line blockquote with a cite reference:

> People think focus means saying yes to the thing you've got to focus on. But that's not what it means at all. It means saying no to the hundred other good ideas that there are. You have to pick carefully. I'm actually as proud of the things we haven't done as the things I have done. Innovation is saying no to 1,000 things.

<cite>Steve Jobs</cite> --- Apple Worldwide Developers' Conference, 1997
{: .small}

```markdown
> People think focus means saying yes to the thing you've got to focus on. But that's not what it means at all. It means saying no to the hundred other good ideas that there are. You have to pick carefully. I'm actually as proud of the things we haven't done as the things I have done. Innovation is saying no to 1,000 things.

<cite>Steve Jobs</cite> --- Apple Worldwide Developers' Conference, 1997
{: .small}
```

## Tables

| Employee         | Salary |                                                              |
| --------         | ------ | ------------------------------------------------------------ |
| [John Doe](#)    | $1     | Because that's all Steve Jobs needed for a salary.           |
| [Jane Doe](#)    | $100K  | For all the blogging she does.                               |
| [Fred Bloggs](#) | $100M  | Pictures are worth a thousand words, right? So Jane × 1,000. |
| [Jane Bloggs](#) | $100B  | With hair like that?! Enough said.                           |

```markdown
| Employee         | Salary |                                                              |
| --------         | ------ | ------------------------------------------------------------ |
| [John Doe](#)    | $1     | Because that's all Steve Jobs needed for a salary.           |
| [Jane Doe](#)    | $100K  | For all the blogging she does.                               |
| [Fred Bloggs](#) | $100M  | Pictures are worth a thousand words, right? So Jane × 1,000. |
| [Jane Bloggs](#) | $100B  | With hair like that?! Enough said.                           |
```

| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|-----------------------------|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=============================|
| Foot1   | Foot2   | Foot3   |

```markdown
| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|-----------------------------|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=============================|
| Foot1   | Foot2   | Foot3   |
```

## Definition Lists

Definition List Title
:   Definition list division.

Startup
:   A startup company or startup is a company or temporary organization designed to search for a repeatable and scalable business model.

#dowork
:   Coined by Rob Dyrdek and his personal body guard Christopher "Big Black" Boykins, "Do Work" works as a self motivator, to motivating your friends.

Do It Live
:   I'll let Bill O'Reilly [explain](https://www.youtube.com/watch?v=O_HyZ5aW76c "We'll Do It Live") this one.

```markdown
Definition List Title
:   Definition list division.

Startup
:   A startup company or startup is a company or temporary organization designed to search for a repeatable and scalable business model.

#dowork
:   Coined by Rob Dyrdek and his personal body guard Christopher "Big Black" Boykins, "Do Work" works as a self motivator, to motivating your friends.

Do It Live
:   I'll let Bill O'Reilly [explain](https://www.youtube.com/watch?v=O_HyZ5aW76c "We'll Do It Live") this one.
```

## Unordered Lists (Nested)

  * List item one 
      * List item one 
          * List item one
          * List item two
          * List item three
          * List item four
      * List item two
      * List item three
      * List item four
  * List item two
  * List item three
  * List item four

```markdown
  * List item one 
      * List item one 
          * List item one
          * List item two
          * List item three
          * List item four
      * List item two
      * List item three
      * List item four
  * List item two
  * List item three
  * List item four
```

## Ordered List (Nested)

  1. List item one 
      1. List item one 
          1. List item one
          2. List item two
          3. List item three
          4. List item four
      2. List item two
      3. List item three
      4. List item four
  2. List item two
  3. List item three
  4. List item four

```markdown
  1. List item one 
      1. List item one 
          1. List item one
          2. List item two
          3. List item three
          4. List item four
      2. List item two
      3. List item three
      4. List item four
  2. List item two
  3. List item three
  4. List item four
```

## Combining Ordered and Unordered Lists

### Ordered -- Unordered -- Ordered

1. ordered item
2. ordered item 
  * **unordered**
  * **unordered** 
    1. ordered item
    2. ordered item
3. ordered item
4. ordered item

```markdown
1. ordered item
2. ordered item 
  * **unordered**
  * **unordered** 
    1. ordered item
    2. ordered item
3. ordered item
4. ordered item
```

### Ordered -- Unordered -- Unordered

1. ordered item
2. ordered item 
  * **unordered**
  * **unordered** 
    * unordered item
    * unordered item
3. ordered item
4. ordered item

```markdown
1. ordered item
2. ordered item 
  * **unordered**
  * **unordered** 
    * unordered item
    * unordered item
3. ordered item
4. ordered item
```

### Unordered -- Ordered -- Unordered

* unordered item
* unordered item 
  1. ordered
  2. ordered 
    * unordered item
    * unordered item
* unordered item
* unordered item

```markdown
* unordered item
* unordered item 
  1. ordered
  2. ordered 
    * unordered item
    * unordered item
* unordered item
* unordered item
```

### Unordered -- Unordered -- Ordered

* unordered item
* unordered item 
  * unordered
  * unordered 
    1. **ordered item**
    2. **ordered item**
* unordered item
* unordered item

```markdown
* unordered item
* unordered item 
  * unordered
  * unordered 
    1. **ordered item**
    2. **ordered item**
* unordered item
* unordered item
```

## Task Lists

- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request
  - [ ] Follow discussions
  - [x] Push new commits

```markdown
- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request
  - [ ] Follow discussions
  - [x] Push new commits
```

## Forms

<form>
  <fieldset>
    <legend>Personalia:</legend>
    Name: <input type="text" size="30"><br>
    Email: <input type="text" size="30"><br>
    Date of birth: <input type="text" size="10">
  </fieldset>
</form>
<br />

```html
<form>
  <fieldset>
    <legend>Personalia:</legend>
    Name: <input type="text" size="30"><br>
    Email: <input type="text" size="30"><br>
    Date of birth: <input type="text" size="10">
  </fieldset>
</form>
```

## Buttons

Make any link standout more when applying the `.btn` class.

```html
<a href="#" class="btn--success">Success Button</a>
```

[Default Button](#){: .btn}
[Primary Button](#){: .btn .btn--primary}
[Success Button](#){: .btn .btn--success}
[Warning Button](#){: .btn .btn--warning}
[Danger Button](#){: .btn .btn--danger}
[Info Button](#){: .btn .btn--info}
[Inverse Button](#){: .btn .btn--inverse}
[Light Outline Button](#){: .btn .btn--light-outline}

```markdown
[Default Button Text](#link){: .btn}
[Primary Button Text](#link){: .btn .btn--primary}
[Success Button Text](#link){: .btn .btn--success}
[Warning Button Text](#link){: .btn .btn--warning}
[Danger Button Text](#link){: .btn .btn--danger}
[Info Button Text](#link){: .btn .btn--info}
[Inverse Button](#link){: .btn .btn--inverse}
[Light Outline Button](#link){: .btn .btn--light-outline}
```

[X-Large Button](#){: .btn .btn--primary .btn--x-large}
[Large Button](#){: .btn .btn--primary .btn--large}
[Default Button](#){: .btn .btn--primary }
[Small Button](#){: .btn .btn--primary .btn--small}

```markdown
[X-Large Button](#link){: .btn .btn--primary .btn--x-large}
[Large Button](#link){: .btn .btn--primary .btn--large}
[Default Button](#link){: .btn .btn--primary }
[Small Button](#link){: .btn .btn--primary .btn--small}
```

## Notices

A notice displays information that explains nearby content. Often used to call attention to a particular detail.

When using Kramdown `{: .notice}` can be added after a sentence to assign the `.notice` to the `<p></p>` element.

### General Notice

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice}` class.
{: .notice}

```markdown
**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice}` class.
{: .notice}
```

### Primary Notice

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--primary}` class.
{: .notice--primary}

```markdown
**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--primary}` class.
{: .notice--primary}
```

### Info Notice

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--info}` class.
{: .notice--info}

```markdown
**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--info}` class.
{: .notice--info}
```

### Warning Notice

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--warning}` class.
{: .notice--warning}

```markdown
**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--warning}` class.
{: .notice--warning}
```

### Danger Notice

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--danger}` class.
{: .notice--danger}

```markdown
**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--danger}` class.
{: .notice--danger}
```

### Success Notice

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--success}` class.
{: .notice--success}

```markdown
**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--success}` class.
{: .notice--success}
```

### Multiple Paragraph or Element Notice

#### Using Liquid and markdownify

{% capture notice-2 %}
**New Site Features**

* You can now have cover images on blog pages
* Drafts will now auto-save while writing
{% endcapture %}

<div class="notice">
  {{ notice-2 | markdownify }}
</div>

```html
{% raw %}{% capture notice-2 %}
#### New Site Features

* You can now have cover images on blog pages
* Drafts will now auto-save while writing
{% endcapture %}{% endraw %}

<div class="notice">{% raw %}{{ notice-2 | markdownify }}{% endraw %}</div>
```

#### Using HTML

<div class="notice">
  <h4>Message</h4>
  <p>A basic message.</p>
</div>

```html
<div class="notice">
  <h4>Message</h4>
  <p>A basic message.</p>
</div>
```

### Notice with Code Block

<div class="notice--primary" markdown="1">
**Primary Notice with code block:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. [Praesent libero](#). Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet.

```html
<html>
  <body>Some body.<body>
</html>
```
</div>

## HTML Tags

### Address Tag

<address>
  1 Infinite Loop<br /> Cupertino, CA 95014<br /> United States
</address>

```html
<address>
  1 Infinite Loop<br /> Cupertino, CA 95014<br /> United States
</address>
```

### Anchor Tag (aka. Link)

This is an example of an external [link](http://apple.com "Apple").

```markdown
[link](http://apple.com "Apple")
```

This is an example of a link to

### Abbreviation Tag

The abbreviation CSS stands for "Cascading Style Sheets".

*[CSS]: Cascading Style Sheets

```markdown
The abbreviation CSS stands for "Cascading Style Sheets".

*[CSS]: Cascading Style Sheets
```

### Cite Tag

"Code is poetry." ---<cite>Automattic</cite>

```html
<cite>Automattic</cite>
```

### Code Tag

You will learn later on in these tests that `word-wrap: break-word;` will be your best friend.

```css
`word-wrap: break-word;`
```

### Strike Tag

This tag will let you <strike>strikeout text</strike>.

```html
<strike>strikeout text</strike>
```

### Emphasize Tag

The emphasize tag should _italicize_ text.

```markdown
_italicize_
```

### Insert Tag

This tag should denote <ins>inserted</ins> text.

```html
<ins>inserted</ins>
```

### Keyboard Tag

This scarcely known tag emulates <kbd>keyboard text</kbd>, which is usually styled like the `<code>` tag.

```html
<kbd>keyboard text</kbd>
```

### Preformatted Tag

This tag styles large blocks of code.

<pre>
.post-title {
  margin: 0 0 5px;
  font-weight: bold;
  font-size: 38px;
  line-height: 1.2;
  and here's a line of some really, really, really, really long text, just to see how the PRE tag handles it and to find out how it overflows;
}
</pre>

```html
<pre>
.post-title {
  margin: 0 0 5px;
  font-weight: bold;
  font-size: 38px;
  line-height: 1.2;
  and here's a line of some really, really, really, really long text, just to see how the PRE tag handles it and to find out how it overflows;
}
</pre>
```

### Quote Tag

<q>Developers, developers, developers&#8230;</q> &#8211;Steve Ballmer

```html
<q>Developers, developers, developers&#8230;</q> &#8211;Steve Ballmer
```

### Strong Tag

This tag shows **bold text**.

```markdown
**bold text**
```

### Subscript Tag

Getting our science styling on with H<sub>2</sub>O, which should push the "2" down.

```html
H<sub>2</sub>O
```

### Superscript Tag

Still sticking with science and Albert Einstein's E = MC<sup>2</sup>, which should lift the 2 up.

```html
E = MC<sup>2</sup>
```

### Variable Tag

This allows you to denote <var>variables</var>.

```html
<var>variables</var>
```

## Text Alignment

### Default

This is a paragraph. It should not have any alignment of any kind. It should just flow like you would normally expect. Nothing fancy. Just straight up text, free flowing, with love. Completely neutral and not picking a side or sitting on the fence. It just is. It just freaking is. It likes where it is. It does not feel compelled to pick a side. Leave him be. It will just be better that way. Trust me.

### Left Align

This is a paragraph. It is left aligned. Because of this, it is a bit more liberal in it's views. It's favorite color is green. Left align tends to be more eco-friendly, but it provides no concrete evidence that it really is. Even though it likes share the wealth evenly, it leaves the equal distribution up to justified alignment.
{: style="text-align: left;"}

```css
This is a paragraph. It is left aligned. Because of this, it is a bit more liberal in it's views. It's favorite color is green. Left align tends to be more eco-friendly, but it provides no concrete evidence that it really is. Even though it likes share the wealth evenly, it leaves the equal distribution up to justified alignment.
{: style="text-align: left;"}
```

### Center Align

This is a paragraph. It is center aligned. Center is, but nature, a fence sitter. A flip flopper. It has a difficult time making up its mind. It wants to pick a side. Really, it does. It has the best intentions, but it tends to complicate matters more than help. The best you can do is try to win it over and hope for the best. I hear center align does take bribes.
{: style="text-align: center;"}

```css
This is a paragraph. It is center aligned. Center is, but nature, a fence sitter. A flip flopper. It has a difficult time making up its mind. It wants to pick a side. Really, it does. It has the best intentions, but it tends to complicate matters more than help. The best you can do is try to win it over and hope for the best. I hear center align does take bribes.
{: style="text-align: center;"}
```

### Right Align

This is a paragraph. It is right aligned. It is a bit more conservative in it's views. It's prefers to not be told what to do or how to do it. Right align totally owns a slew of guns and loves to head to the range for some practice. Which is cool and all. I mean, it's a pretty good shot from at least four or five football fields away. Dead on. So boss.
{: style="text-align: right;"}

```css
This is a paragraph. It is right aligned. It is a bit more conservative in it's views. It's prefers to not be told what to do or how to do it. Right align totally owns a slew of guns and loves to head to the range for some practice. Which is cool and all. I mean, it's a pretty good shot from at least four or five football fields away. Dead on. So boss.
{: style="text-align: right;"}
```

### Justify Align

This is a paragraph. It is justify aligned. It gets really mad when people associate it with Justin Timberlake. Typically, justified is pretty straight laced. It likes everything to be in it's place and not all cattywampus like the rest of the aligns. I am not saying that makes it better than the rest of the aligns, but it does tend to put off more of an elitist attitude.
{: style="text-align: justify;"}

```css
This is a paragraph. It is justify aligned. It gets really mad when people associate it with Justin Timberlake. Typically, justified is pretty straight laced. It likes everything to be in it's place and not all cattywampus like the rest of the aligns. I am not saying that makes it better than the rest of the aligns, but it does tend to put off more of an elitist attitude.
{: style="text-align: justify;"}
```

## Image Alignment

### Center Align

![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-580x300.jpg){: .align-center}

The image above happens to be **centered**.

```markdown
{% raw %}![image-center]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-580x300.jpg){: .align-center}{% endraw %}
```

### Align Left

![image-left]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-150x150.jpg){: .align-left} The rest of this paragraph is filler for the sake of seeing the text wrap around the 150×150 image, which is **left aligned**.

As you can see the should be some space above, below, and to the right of the image. The text should not be creeping on the image. Creeping is just not right. Images need breathing room too. Let them speak like you words. Let them do their jobs without any hassle from the text. In about one more sentence here, we'll see that the text moves from the right of the image down below the image in seamless transition. Again, letting the do it's thing. Mission accomplished!

```markdown
{% raw %}![image-left]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-150x150.jpg){: .align-left} The rest of this paragraph is filler for the sake of seeing the text wrap around the 150×150 image, which is **left aligned**.

As you can see the should be some space above, below, and to the right of the image. The text should not be creeping on the image. Creeping is just not right. Images need breathing room too. Let them speak like you words. Let them do their jobs without any hassle from the text. In about one more sentence here, we'll see that the text moves from the right of the image down below the image in seamless transition. Again, letting the do it's thing. Mission accomplished!{% endraw %}
```

### Right Align

![image-right]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-300x200.jpg){: .align-right}

And now we're going to shift things to the **right align**. Again, there should be plenty of room above, below, and to the left of the image. Just look at him there --- Hey guy! Way to rock that right side. I don't care what the left aligned image says, you look great. Don't let anyone else tell you differently.

In just a bit here, you should see the text start to wrap below the right aligned image and settle in nicely. There should still be plenty of room and everything should be sitting pretty. Yeah --- Just like that. It never felt so good to be right.

```markdown
{% raw %}![image-right]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-300x200.jpg){: .align-right}

And now we're going to shift things to the **right align**. Again, there should be plenty of room above, below, and to the left of the image. Just look at him there --- Hey guy! Way to rock that right side. I don't care what the left aligned image says, you look great. Don't let anyone else tell you differently.

In just a bit here, you should see the text start to wrap below the right aligned image and settle in nicely. There should still be plenty of room and everything should be sitting pretty. Yeah --- Just like that. It never felt so good to be right.{% endraw %}
```

### Large Image with No Align

![no-alignment]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-1200x4002.jpg)

The image above, though 1200px wide, should not overflow the content area. It should remain contained with no visible disruption to the flow of content.

```markdown
{% raw %}![no-alignment]({{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-1200x4002.jpg)

The image above, though 1200px wide, should not overflow the content area. It should remain contained with no visible disruption to the flow of content.{% endraw %}
```

### Center Align with Caption

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-580x300.jpg" alt="">
  <figcaption>Look at 580 x 300 getting some love.</figcaption>
</figure> 

The figure above happens to be **centered**. The caption also has a link in it, just to see if it does anything funky.

```markdown
{% raw %}<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-580x300.jpg" alt="">
  <figcaption>Look at 580 x 300 getting some love.</figcaption>
</figure> 

The figure above happens to be **centered**. The caption also has a link in it, just to see if it does anything funky.
{% endraw %}
```

### Left Align with Caption

<figure style="width: 150px" class="align-left">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-150x150.jpg" alt="">
  <figcaption>Itty-bitty caption.</figcaption>
</figure> 

The rest of this paragraph is filler for the sake of seeing the text wrap around the 150×150 image, which is **left aligned**.

As you can see the should be some space above, below, and to the right of the image. The text should not be creeping on the image. Creeping is just not right. Images need breathing room too. Let them speak like you words. Let them do their jobs without any hassle from the text. In about one more sentence here, we'll see that the text moves from the right of the image down below the image in seamless transition. Again, letting the do it's thing. Mission accomplished!

```html
{% raw %}<figure style="width: 150px" class="align-left">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-150x150.jpg" alt="">
  <figcaption>Itty-bitty caption.</figcaption>
</figure> 

The rest of this paragraph is filler for the sake of seeing the text wrap around the 150×150 image, which is **left aligned**.

As you can see the should be some space above, below, and to the right of the image. The text should not be creeping on the image. Creeping is just not right. Images need breathing room too. Let them speak like you words. Let them do their jobs without any hassle from the text. In about one more sentence here, we'll see that the text moves from the right of the image down below the image in seamless transition. Again, letting the do it's thing. Mission accomplished!{% endraw %}
```

### Right Align with Caption

<figure style="width: 300px" class="align-right">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-300x200.jpg" alt="">
  <figcaption>Feels good to be right all the time.</figcaption>
</figure> 

And now we're going to shift things to the **right align**. Again, there should be plenty of room above, below, and to the left of the image. Just look at him there --- Hey guy! Way to rock that right side. I don't care what the left aligned image says, you look great. Don't let anyone else tell you differently.

In just a bit here, you should see the text start to wrap below the right aligned image and settle in nicely. There should still be plenty of room and everything should be sitting pretty. Yeah --- Just like that. It never felt so good to be right.

```html
{% raw %}<figure style="width: 300px" class="align-right">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-300x200.jpg" alt="">
  <figcaption>Feels good to be right all the time.</figcaption>
</figure> 

And now we're going to shift things to the **right align**. Again, there should be plenty of room above, below, and to the left of the image. Just look at him there --- Hey guy! Way to rock that right side. I don't care what the left aligned image says, you look great. Don't let anyone else tell you differently.

In just a bit here, you should see the text start to wrap below the right aligned image and settle in nicely. There should still be plenty of room and everything should be sitting pretty. Yeah --- Just like that. It never felt so good to be right.{% endraw %}
```

### Oversized Image with Caption

<figure style="width: 1200px">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-1200x4002.jpg" alt="">
  <figcaption>Massive image comment for your eyeballs.</figcaption>
</figure> 

The figure element above has an inline style of `width: 1200px` set which should break it outside of the normal content flow.

```html
{% raw %}<figure style="width: 1200px">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-1200x4002.jpg" alt="">
  <figcaption>Massive image comment for your eyeballs.</figcaption>
</figure> 

The figure element above has an inline style of `width: 1200px` set which should break it outside of the normal content flow.{% endraw %}
```

### Oversized Image Bound by Content Area with Caption

<figure>
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-1200x4002.jpg" alt="">
  <figcaption>Image resized for your viewing pleasure.</figcaption>
</figure> 

The figure element above has no style set. It should be bound by the content area.

```html
{% raw %}<figure>
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/styleguide/image-alignment-1200x4002.jpg" alt="">
  <figcaption>Image resized for your viewing pleasure.</figcaption>
</figure> 

The figure element above has no style set. It should be bound by the content area.{% endraw %}
```
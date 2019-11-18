---
title: Functions Available
date: 2019-10-24 23:30:09
updated: 2019-11-03 15:11:04
tags: [Foo, Bar]
categories: [Baz, Foo]
---

This post contains most of the functions in a post that are suuported by jekyll.

<!-- more -->

# Post type

## A post with description:

{% highlight yml %}
---
title: Link Post
date: 2013-12-24 23:30:04
description: Gallery Post Test.
---
{% endhighlight %}

## A post with categories and tags:

{% highlight yml %}
---
title: Link Post
date: 2013-12-24 23:30:04
categories:
- Foo
- Bar
tags:
- Foo
- Baz
---
{% endhighlight %}

or more elegant:

{% highlight yml %}
---
title: Link Post
date: 2013-12-24 23:30:04
categories: [Foo, Bar]
tags: [Foo, Baz]
---
{% endhighlight %}

or if there's only one(optional): 

{% highlight yml %}
---
title: Link Post
date: 2013-12-24 23:30:00
category: Foo
tag: Baz
---
{% endhighlight %}

## A post with updated time:

{% highlight yml %}
---
title: Updated post
tags: post
date: 2017-07-20
updated: 2019-11-03 15:11:04
---
{% endhighlight %}

The `updated` and `date` section can be only date without specific time.

## A link post example: 

{% highlight yml %}
---
title: Link Post
date: 2013-12-24 23:30:04
link: http://www.google.com/
categories:
- Foo
---
{% endhighlight %}

## A gallery post example:

{% highlight yml %}
---
type: photo
title: Gallery Post
date: 2014-11-18 15:45:20
limit: 8
---
{% endhighlight %}

## A picture post example:

{% highlight yml %}
---
type: picture
title: Picture post
---
{% endhighlight %}

After `front-matter`, post should include an image element. Text is allowed and is optional.

{% highlight yml %}
![Wallbase](https://files.ericy.me/2015/07/20150719_120307.jpg)
{% endhighlight %}

# Emoji test:

This is an emoji test. :smile: lol.

See emoji cheat sheet for more detail :wink: : <https://www.webpagefx.com/tools/emoji-cheat-sheet/>.

:bowtie::smile::laughing::blush::smiley::relaxed::smirk:
:heart_eyes::kissing_heart::kissing_closed_eyes::flushed::relieved::satisfied::grin:

# Math equations

Inline equations: $\sqrt{\frac{n!}{k!(n-k)!}}$, and Block equations:

$$a^2 + b^2 = c^2$$


# Code blocks

## Block Quote

### Normal blockquote

> Praesent diam elit, interdum ut pulvinar placerat, imperdiet at magna.

## Code Block

### Inline code block

This is a inline code block: `python`, `print 'helloworld'`.

### Normal code block

```
alert('Hello World!');
```

    print "Hello world"

### Highlight code block

```python
print "Hello world"
```

{% highlight ruby %}
def foo
  puts 'foo'
end
{% endhighlight %}

{% highlight ruby linenos %}
def foo
  puts 'foo'
end
{% endhighlight %}

### Gist

{% gist 996818 %}

# Markdown Elements

The purpose of this post is to help you make sure all of HTML elements can display properly. If you use CSS reset, don't forget to redefine the style by yourself.

---

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

---

## Paragraph

Lorem ipsum dolor sit amet, [test link]() consectetur adipiscing elit. **Strong text** pellentesque ligula commodo viverra vehicula. *Italic text* at ullamcorper enim. Morbi a euismod nibh. <u>Underline text</u> non elit nisl. ~~Deleted text~~ tristique, sem id condimentum tempus, metus lectus venenatis mauris, sit amet semper lorem felis a eros. Fusce egestas nibh at sagittis auctor. Sed ultricies ac arcu quis molestie. Donec dapibus nunc in nibh egestas, vitae volutpat sem iaculis. Curabitur sem tellus, elementum nec quam id, fermentum laoreet mi. Ut mollis ullamcorper turpis, vitae facilisis velit ultricies sit amet. Etiam laoreet dui odio, id tempus justo tincidunt id. Phasellus scelerisque nunc sed nunc ultricies accumsan.

Interdum et malesuada fames ac ante ipsum primis in faucibus. `Sed erat diam`, blandit eget felis aliquam, rhoncus varius urna. Donec tellus sapien, sodales eget ante vitae, feugiat ullamcorper urna. Praesent auctor dui vitae dapibus eleifend. Proin viverra mollis neque, ut ullamcorper elit posuere eget.

> Praesent diam elit, interdum ut pulvinar placerat, imperdiet at magna.

Maecenas ornare arcu at mi suscipit, non molestie tortor ultrices. Aenean convallis, diam et congue ultricies, erat magna tincidunt orci, pulvinar posuere mi sapien ac magna. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Praesent vitae placerat mauris. Nullam laoreet ante posuere tortor blandit auctor. Sed id ligula volutpat leo consequat placerat. Mauris fermentum dolor sed augue malesuada sollicitudin. Vivamus ultrices nunc felis, quis viverra orci eleifend ut. Donec et quam id urna cursus posuere. Donec elementum scelerisque laoreet.

## List Types

### Definition List (dl)

<dl><dt>Definition List Title</dt><dd>This is a definition list division.</dd></dl>

### Ordered List (ol)

1. List Item 1
2. List Item 2
3. List Item 3

### Unordered List (ul)

- List Item 1
- List Item 2
- List Item 3

## Table

| Table Header 1 | Table Header 2 | Table Header 3 |
| --- | --- | --- |
| Division 1 | Division 2 | Division 3 |
| Division 1 | Division 2 | Division 3 |
| Division 1 | Division 2 | Division 3 |

## Footnote

NexT is a high quality [^highquality] elegant [Jekyll](https://jekyllrb.com) theme ported from [Hexo Next](https://github.com/iissnan/hexo-theme-next). It is crafted from scratch, with love.

[^highquality]: Test footnote, [Link](https://google.com).

## Image

![Desktop Sidebar Preview](/assets/images/theme/navbg.jpg)

![Wallbase3](https://files.ericy.me/2015/07/20150719_120307.jpg)

## Iframe - Y2B, Gist etc.

<iframe width="560" height="315" src="https://www.youtube.com/embed/shPvWBx9pfQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<script src="https://gist.github.com/ericworks/f7276fbbacf773d58d073339107a2a61.js"></script>

## Misc Stuff - abbr, acronym, sub, sup, etc.

Lorem <sup>superscript</sup> dolor <sub>subscript</sub> amet, consectetuer adipiscing elit. Nullam dignissim convallis est. Quisque aliquam. <cite>cite</cite>. Nunc iaculis suscipit dui. Nam sit amet sem. Aliquam libero nisi, imperdiet at, tincidunt nec, gravida vehicula, nisl. Praesent mattis, massa quis luctus fermentum, turpis mi volutpat justo, eu volutpat enim diam eget metus. Maecenas ornare tortor. Donec sed tellus eget sapien fringilla nonummy. <acronym title="National Basketball Association">NBA</acronym> Mauris a ante. Suspendisse quam sem, consequat at, commodo vitae, feugiat in, nunc. Morbi imperdiet augue quis tellus.  <abbr title="Avenue">AVE</abbr>

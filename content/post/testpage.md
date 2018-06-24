---
title: "Testpage"
date: 2018-06-20T14:26:59+07:00
lastmod: 2018-06-20T14:26:59+07:00
draft: false
keywords: ["Testing", "Hugo"]
description: ""
tags: ["Rant", "Markdown", "Mathjax", "Hugo"]
categories: ["Uncategorized"]
author: "Hagun"

# You can also close(false) or open(true) something for this content.
# P.S. comment can only be closed
comment: false
toc: true
autoCollapseToc: false
postMetaInFooter: false
hiddenFromHomePage: false
# You can also define another contentCopyright. e.g. contentCopyright: "This is another copyright."
contentCopyright: false
reward: false
mathjax: true
mathjaxEnableSingleDollar: true
mathjaxEnableAutoNumber: false

# You unlisted posts you might want not want the header or footer to show
hideHeaderAndFooter: false
---
# Just a test page
It's been a long time since I've been looking for a solution for my blog.
A CMS is easy to use but it requires dedicated server and I didn't want that.
After searching for a while, I went with static page.

It's a little steep learning curve for an electrical student, but the result is worth the effort.

I just want to test some functions for my blog, so this post come first.

# Markdown
Hugo uses Black Friday Markdown Parser which support Github-flavored Markdown. For the test, I would like to test all the features of Github-flavored Markdown. I refered to [this page](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for the markdown.

After pasting the Markdown and see the result, everything is working perfectly. The only thing not working is the Header underline and triple or more "=". I have inspected the headers but there is no (underline) element. There is no Hugo's option with Black Friday for header underline, but it's okay, I don't think the underline is pretty, though.

## Test
I leave some test for later convenience.

Emphasis, aka italics, with *asterisks* or _underscores_.
Strong emphasis, aka bold, with **asterisks** or __underscores__.
Combined emphasis with **asterisks and _underscores_**.
Strikethrough uses two tildes. ~~Scratch this.~~

===

---

1. First ordered list item
2. Another item
    * Unordered sub-list. 
3. Actual numbers don't matter, just that it's a number
    1. Ordered sub-list (4 spaces)
        - 4 spaces again
4. And another item.

    You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

    To have a line break without a paragraph, you will need to use two trailing spaces.  
    Note that this line is separate, but within the same paragraph.  
    (This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

Inline `code` has `back-ticks` around it.

```javascript
Even.backToTop = function () {
  const $backToTop = $('#back-to-top')

  $(window).scroll(function () {
    if ($(window).scrollTop() > 100) {
      $backToTop.fadeIn(1000)
    } else {
      $backToTop.fadeOut(1000)
    }
  })

  $backToTop.click(function () {
    $('body,html').animate({ scrollTop: 0 })
  })
}
```

```python
s = "Python syntax highlighting"
print s
```

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```

# Mathjax
Hugo suggests that Latex's underscores may cause Markdown confuse. But after testing some simple case, I didn't find anything wrong with my pages.

Test underscores `x_1=x_2`: $x_1=x_2$

Mathblock:
$$\lim_{x\to 0}x = 0$$

Inline: $\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$

Use argmax without declare: `\underset{x}{\operatorname{arg\,max}}`
$$\underset{x}{\operatorname{arg\,max}} x+1 = \infty$$
Declare argmin: `\DeclareMathOperator*{\argmin}{arg\,min}`

$$\DeclareMathOperator*{\argmin}{arg\,min}$$

$$\argmin_{x}x^2 = 0$$

Something more complex:
$$f\left(\argmin_xf(x)\right) = \min_xf(x)$$

I wouldn't use more complex case much, so maybe it's good enough.

# Conclusion
The theme (Even) is working perfect, Hugo is working perfect, Markdown, Mathjax is flawless.

Thank you all.

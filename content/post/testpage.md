---
title: "Testpage"
date: 2018-06-20T14:26:59+07:00
lastmod: 2018-06-20T14:26:59+07:00
draft: false
keywords: ["Testing", "Hugo"]
description: ""
tags: ["Rant", "Markdown", "Mathjax", "Hugo"]
categories: []
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

# You can enable or disable out-of-date content warning for individual post.
# Comment this out to use the global config.
#enableOutdatedInfoWarning: false

flowchartDiagrams:
  enable: false
  options: ""

sequenceDiagrams: 
  enable: false
  options: ""

---
# Just a test page
A long time since I've been looking for a solution for my blog.
CMS is easy to use but it requires dedicated server and I didn't want that.
So static page, here I come.

It's a little steep learning curve for an electrical student, but the result is worth the effort.

I just want to test some functions for my blog, so this post come first.

# Markdown
As Hugo uses Black Friday Markdown Parser, I want to check what can it do. I have a quick look at Black Friday's Github Repo, and I see there is Github-flavored Markdown.

For the test, I would like to test all the features of Github-flavored Markdown. I refered to [this page](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for the markdown.

After pasting the Markdown and see the result, everything is working perfectly. The only thing not working is the Header underline (triple or more "=" and "-"). I have inspected the headers but there is no (underline) element. There is no Hugo's option with Black Friday for header underline, but it's okay, I don't want that (ugly) underline, though.

# Mathjax
Hugo suggests that Latex's underscores may cause Markdown confuse. But after testing some simple case, I didn't find anything wrong with my pages.

Mathblock:
$$x+y$$

Inline: $x_1-y=f(x^2)$

Something more complex: $$\underset{x}{argmax}f(x) = \frac{x_1+x_2+...+x_n}{y}$$

I didn't use much more complex case so maybe it's good enough.

# Conclusion
The theme (Even) is working perfect, Hugo is working perfect, Markdown, Mathjax is flawless.

Thank you all.

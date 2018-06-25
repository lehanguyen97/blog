---
title: "Create a Blog"
date: 2018-06-24T22:11:22+07:00
lastmod: 2018-06-24T22:11:22+07:00
draft: false
keywords: ["Hosting", "Static Site Generator", "Github Pages"]
description: "Journey for hosting a blog"
tags: ["Rant", "Hugo", "Even", "Github Pages"]
categories: ["Experience"]
author: "Hagun"

comment: true
toc: true
autoCollapseToc: false
postMetaInFooter: false
hiddenFromHomePage: false
# You can also define another contentCopyright. e.g. contentCopyright: "This is another copyright."
contentCopyright: false
reward: false
mathjax: false
mathjaxEnableSingleDollar: false
mathjaxEnableAutoNumber: false

hideHeaderAndFooter: false
---


# Welcome
> Warning: Rant, Noob

Just to let you know, I'm not a web designer or developer.
I'm a normal (poor) electronics student who haven't got a credit card.

To have this blog being read by someone other than myself, in my opinion, is a hard work.
My goal is to host a simple website where I can write something to keep myself being motivated.

I wouldn't want to spend money on hosting, it's not because I want everything free but because I think there is some way I can do it and I want some more food each month.

I've been through Wordpress and Heroku, looking at GatsbyJS for new tech, and here I am with Hugo.

# Time with Wordpress
I'm not a web developer or have a lot of experience in it.
But I did several projects which require server and web UI for IoT, mainly write in PHP, Bootstrap, and JQuery.
The main focus of these project is the board (MCU) and protocol like WebSocket or MQTT.

## 000Webhost
So I went back to [000Webhost](https://www.000webhost.com/), where I hosted a project last time, created a server and setup Wordpress.
It was an easy time setup and using a mature software like Wordpress.
The only thing I have to deal with is working with Markdown (at the end, I use Jetpack).
Everything else from theme to manage comment, post is done in GUI and is super easy.

But 000Webhost have sleep time, and (very) slow connection, plus Wordpress being heavy.
The user experience is not so good. I only open 2 tabs and have to wait for 1'.
Don't know what will happen when I have like 10 peoples visit.

So, I went on my way finding another free hosting service.
A lot of good reviews free hosting service do not allow Viet Nam IP, other sites are just scam. It took me a lot of time registering and got back nothing but depression and spam email.

## Byethost
At last, I found [Byethost](https://byet.host/), very promise hosting site: unlimited bandwidth, 20 free SQL, better connection,...
Everything happens smoothly until I messed up with file permission, my Wordpress could not set admin password.
I've set everything to *777*, reinstalled everything to reset permission, but the problem still persists.
After retried for like 20 times, it worked.
I went through customize theme (Hestia, after trying Hueman at 000Webhost) and boom, CSS or something is not working most of the time, like with the admin password, leave the website with a 90s theme.

## Leaving
So depressed, I'd thought of using [Wordpress.com](https://wordpress.com/) free plan (with ads) or register a VISA and go with AWS, Azure or Digital Ocean.


# Heroku and Ghost
After wandering around Stack Overflow, Quora,... I found [Ghost](https://ghost.org/), a beautiful blog platform.
It can be self-hosted with Node JS server. 
I went with [Heroku](https://www.heroku.com/) after found some guide to hosting Ghost on Heroku's free plan.
But the bad news comes when I start working with database.
The only free database work without credit-card verification is Postgres which support has been drop by Ghost.

Heroku also has sleep time and some limit which I don't like too.
But I'm not blaming them for such a great free service.

Well, it's not easy to get some free-service without identity.

# Static site and Github
I just so frustrated at that time, I didn't want to create this blog anymore.
I would write some Markdown file with VS Code and lets my head not being filled with those things.

And here comes a comment which suggests host Static Site on Github for free.
I've seen some Github Pages (site ends with **github.io**) without knowing about it.

Static Site is a bunch of pages which don't asks server for anything but the data it've been stored.
Perfectly fine with me as long as I have something to keep my post organized (which I use Hugo for).

Github Pages provides a free github.io domain and HTTPS for custom domain.
I considered Gitlab for free privated repo but, it's not important.

## Choosing Static Site Generator
Github offers to build static site with [Jekyll](https://jekyllrb.com/), the most used Static Site Generator (*SSG*).
It's come with a lot of great built-in theme, plugin due to its large user base. I just have to clone then build with Jekyll on my PC.

But I don't like installing Ruby (>100MB) and get a slow building speed.
So I do some finding, again, and found Hugo, Hexo, and Gatsby.

Hexo, Gatsby is written in NodeJS, Hugo is written in Go.
All of them offer less but not half bad theme, docs, support,... and very fast build speed.

When visiting Hexo, I found some 2-year-old comment stayed on top, which let me down a little bit.
Gatsby is a promising one, come which a lot of new shiny technology like GraphQL and React.
But, after following the docs, I found it's too low-level, which means I have to build my blog nearly from scratch.
For electronics student like me, it's somewhat interesting, but, you know, I have my subject and lots of things to learn.

So I go with Hugo and lets Gatsby wait for some more time.

## Hugo and Even Theme
I only need a single executable (17MB) to get a fast SSG and hot-reload web server for testing, fantastic.
Hugo's theme library is not small at all.
I've found lots of good theme in it like [Tranquilpeak](https://github.com/kakawait/hugo-tranquilpeak-theme) or [Sublime Hugo](https://github.com/dt801ts/sublime-hugo-theme).

Currently, I use [Even](https://github.com/olOwOlo/hugo-theme-even), which has the tags and categories I need, besides good Highlight, Table of Content, MathJax,... and responsive design.

To changed some setting, I spent some free day, worked through the docs, reading source code.
Sometimes, it's boring and frustrating.
But in the end, I learned a lot about new JS, SCSS, TOML, YAML, timeago.js, slideout.js, how to manage project file,...

Maybe I'll write something about my work with this theme if I change some more (currently it's only a little change compare to LOC of the original code).

# Thanks
Now, those web knowledge may not be helpful for me.
But knowledge is always a good thing, right?

And guess what? I have a good-looking, functional blog for me to write this post.

Thanks, everyone.

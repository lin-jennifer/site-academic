---
title: 'Websites using Academic: What I Learned and What I Wish I Knew'
author: Jennifer Lin
date: '2020-05-03'
slug: websites-using-academic
categories: ["Documentation"]
tags:
  - R
  - Websites
subtitle: ''
summary: ''
authors: []
lastmod: '2020-05-03'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

The [Academic theme on Hugo](https://themes.gohugo.io/academic/) is quite a popular theme for people, especially academics to use to create their own websites, be it for a lab or as a personal portfolio page, like this one. And this is for a good reason. [Academic](https://sourcethemes.com/academic/) is quite easy to use and it is very flexible to the needs of the user, allowing creators to design web pages using a variety of widgets and even allowing them to create some new ones.

Then, you may ask, why are you writing this post? Well, as the title suggests, there were a few things I learned that I wanted to document for my future self and for those wishing to pick this theme up. Many users have also done something similar, with great examples being from [George Cushen, the creator of Academic](https://georgecushen.com/create-your-website-with-hugo/), and [Allison Hill, a coauthor on Blogdown](https://alison.rbind.io/post/2019-02-21-hugo-page-bundles/). I should note that this post is not necessarily geared towards a setp-by-step on how to create a website using Hugo themes, as those tips are documented by the creators of the themes themselves.

## What I Wish I Knew

Let's begin with the second question because I think it is more straightforward and something that people who want to use this theme should know -- *Academic is so simple, yet complex*.

Given the amount of documentation that Academic and their community of users provide on the internet, it is easy to understand the "*simple*" component. Academic relies on Markdown, or R Markdown if you would prefer. 

But, the more complicated part comes with the organization of the site, which, for beginners, may come with a learning curve. I created my site using [Blogdown](https://bookdown.org/yihui/blogdown/), but there are many ways that one can use to create and deploy an Academic site. But regardless of what you end up choosing, the first few hours, maybe days, would be dedicated to you constantly asking yourself: "*Where is that file?*" The [Blogdown book](https://bookdown.org/yihui/blogdown/), which I recommend looking through if you choose Blogdown, suggests a 10 minute curve for users not familiar with code in CSS or JavaScript, but my personal experience showed that it took a lot longer for me to get accustomed to the site and framework.

However, the good news is that once you get over the learning curve, it is quite easy to edit and innovate your Academic site.

## What I Learned

As I discussed earlier, there can be a learning curve to the site. In the rest of this post, I will attempt to document all the tips I found handy in my process of getting accustomed to the site. In this process, I assume that you are using Blogdown and have [read the book](https://bookdown.org/yihui/blogdown/) to know how to [initiate an Academic site](https://bookdown.org/yihui/blogdown/other-themes.html)[^1]

1. Assuming you don't already know Markdown, learn some basic syntax. Academic's documentation provides a [great guide to do this](https://sourcethemes.com/academic/docs/writing-markdown-latex/). It also helps to have a general understanding of HTML syntax as well.
2. Bookmark some cheat sheets. I recommend:
    1. [Font Awesome general (fas)](https://fontawesome.com/icons?d=gallery&s=regular,solid) and [Font Awesome Brand (fab)](https://fontawesome.com/icons?d=gallery&s=brands)
    2. [Academicons](https://jpswalsh.github.io/academicons/)
    3. [Emojis Cheatsheet](https://www.webfx.com/tools/emoji-cheat-sheet/)
    4. [HTML Symbols Cheatsheet](https://www.toptal.com/designers/htmlarrows/)
3. Build your site often to see if there are errors. I recommend using the `blogdown:::serve_site()` command, which, if you use R Studio, generates a preview in a viewer tab in your screen.
4. Regardless of the approach you use to create and edit your site, ***DO NOT TOUCH*** the `themes/` folder in your site source. You can mirror the file structure under the `themes/` folder to create your own content, as [explained here](https://sourcethemes.com/academic/docs/page-builder/).
5. When building with Blogdown and deplaying to GitHub pages, I recommend using a two repository system where one serves as the `source` and the other is the publish directory. This is because there are some challenges for GitHub pages to get along with Hugo.[^2] For this website, I have a source repository where I make my edits and publish it to my website directory (`lin-jennifer.github.io`). You can use this system by adding `publishDir = "../USERNAME.github.io"` to your `config.toml` file, where `USERNAME` is your GitHub username.

[^1]: All this could be done using point-and-click in R Studio as well. Simply go to `File` &rarr; `New Project` &rarr; `New Directory` &rarr; `Website using Blogdown` and select the options that you want, including `gcushen/hugo-academic` in the theme field to signal Academic as your theme.

[^2]: Hugo provides some guidence on some different ways to deploy to GitHub Pages [here](https://gohugo.io/hosting-and-deployment/hosting-on-github/). However, the two repository system is what I see some users use and what I find to be the most straightforward.

## Going Forward

As I keep saying throughout this piece, there are many ways that one can use, create and edit Academic. If there is something that you know that would make editing and creating content easier, please [let me know](https://lin-jennifer.github.io/#contact)!
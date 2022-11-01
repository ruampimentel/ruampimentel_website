---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Hugo Format Error"
subtitle: ""
summary: ""
authors: [admin]
tags: [hugo, wowchemy]
categories: []
date: 2022-11-01T15:06:29-04:00
lastmod: 2022-11-01T15:06:29-04:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

It took me about 40 min to fix this 'simple' issue. 

The bug below appears for me after updating wowchemy. I use [wowchemy](https://wowchemy.com/) and [hugo](https://gohugo.io/) to run this website.

The essential part of the steps I took to solve this problem came from [Justin Pearson post](https://user.it.uu.se/~justin/Hugo/post/hugo_module_fail/). However, their fix was not enough for me. So I had to find more info.

Other part came from [wowchemy docs](https://wowchemy.com/docs/hugo-tutorials/troubleshooting/#error-failed-to-resolve-output-format).

##  The error

`Error: from config: failed to resolve output format "headers" from
site config`

## The fix
Steps
- Go to `config/_default/config.yaml` file
- change the following line
  
     `home: [HTML, RSS, JSON, WebAppManifest, headers, redirects]`
      
    to

    `home: [] #[HTML, RSS  , JSON, WebAppManifest, headers, redirects]`
- Save the previous change (cmd + s on a Mac)
- Go to your TERMINAL and run `hugo mod get`
- Still in your terminal, clean your cache by running `hugo mod clean --all`
- Go back to `config/_default/config.yaml` file and change the `home:` line back to the original code:
    
     `home: [HTML, RSS, JSON, WebAppManifest, headers, redirects]`
- Save your changes again (Cmd + s on a Mac)
  

Everything might back to normal :D

# Explanation of the problem

Unfortunely, when wowchemy have some updates, sometimes, it doesn't update some features like the ones we saw above. Hence, the old cache creates a bug with the updated version from wowchemy. 

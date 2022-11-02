---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "From R (Rstudio) to Github"
subtitle: "First commit - Sentting up repository"
summary: ""
authors: [admin]
tags: [r, github, git, rstudio]
categories: []
date: 2022-10-28T17:46:09-04:00
lastmod: 2022-10-28T17:46:09-04:00
featured: true
draft: false

show_related: true
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

{{% callout note %}}
I still have to update this post, but the quick tip is:
{{% /callout %}}

When I have to set up a new project connecting Git, GitHub, and Rstudio, I always open Google and type 'How to...' and spend a couple of minutes (sometimes hours) findings the specific info I need. 

Anyway. Here is the easiest path I found to create a GitHub repository and connect with Rstudio when I already created an R project on my computer. 

The step-by-step and full explanation is explained [here](https://happygitwithr.com/existing-github-last.html).

For now, that is the important thing:
  1. Open the Rproject on Rstudio. 
  2. follow the steps below:

```R
# First, setup git for this project with
usethis::use_git()
# Second, send everything to GitHub
usethis::use_github()
```


Bonus tip: use [.gitignore and don't sync entire folder](https://www.educative.io/answers/how-to-add-folder-to-gitignore)

Bonuis tip2: check out git [cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)
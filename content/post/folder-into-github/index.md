---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Folder Into Github"
subtitle: ""
summary: ""
authors: [admin]
tags: [git, github]
categories: []
date: 2022-11-01T15:26:03-04:00
lastmod: 2022-11-01T15:26:03-04:00
featured: false
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

Sometimes,  I want to link a folder from my pc (or mac) with GitHub, and I'm not using Rstudio on that folder. I'm only syncing other kinds of projects with no 'coding' or 'syntax'. 

So here is what you should do:

1. First, we have to turn my directory (i.e., folder) into a git repository. 
2. Then I can link that git repository with GitHub in many ways. 

### Step 1 - Turn a directory into a git repository

You can see the step by step explained [here](https://github.com/git-guides/git-init)

1. Open TERMINAL (on mac).
2. run the code below
    
    `git init <directory>`

    Where it says <directory> you will put the directory path. (e.g., `/Users/ruampimentel/Library/CloudStorage/OneDrive/my-project` )

### Step 2 - connect git repository with github

Then the easist one for me is to do [this](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/adding-and-cloning-repositories/adding-a-repository-from-your-local-computer-to-github-desktop)

- I use GitHub desktop to connect
- Open GitHub desktop
- Go to 'file'
- Select 'Add local Repository...''
- Accept the settings.
- Done ;)



---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Quarto Tips"
subtitle: ""
summary: ""
authors: [admin]
tags: [r, quarto]
categories: []
date: 2022-11-02T12:38:10-04:00
lastmod: 2022-11-02T12:38:10-04:00
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

# Exporting as .docx as APA format
Those are tips and reminders to myself... Enjoy if they are useful for you too. 


Using Quarto (on Rstudio) I can export to a Word document with a specific style.

Example. I can create an APA-7ed-style word file, and export my text, figures, and tables to APA format. 

[Click here](https://quarto.org/docs/output-formats/ms-word-templates.html) to see a tutorial on how to do it. 

[Click here](https://drive.google.com/drive/folders/1eBVPgOClTyuX9uff1po5Vj1tpmXODx76) to see the APA style I've organized. 

## Summary of the tutorial
Basically, you only need:
1. Add the .docx file with the style ([example](https://drive.google.com/drive/folders/1eBVPgOClTyuX9uff1po5Vj1tpmXODx76)) in the same folder as the Quarto file. 
2. Add the following syntax to at the top of the file:

```{r} 
format:  
  docx:
    reference-doc: custom-reference-doc.docx
```
3. Done
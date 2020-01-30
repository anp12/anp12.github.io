---
date: "2020-01-23T00:00:00Z"
draft: false
lastmod: "2020-01-23T00:00:00Z"
linktitle: Principles of Marketing
menu:
  example:
    name: Overview
    weight: 1
summary: Alec Pappas was the instructor of Principles of Marketing during the Summer of 2019. The class had 50 students participate. Alec Pappas received a 4.76/5 rating for the class. Below are a few reviews of Alec from students... "Although he's young and this is his first real teaching experience, Alec is the man. He's very well spoken, makes the material even easier to understand with his examples/dialogue, and actually cares about his students. He has no issues taking the time to thoroughly explain something, and gives the extra effort to his students when needed. He is very well respected by the entire class, he communicates very well, and he's an inspirational/motivative person."      /      "Prof Alec really went above and beyond to educate students. His lecture were clear and effective. It was easy to see that he genuinely cared about educating students. He personally helped me work through questions and was one of the best teachers I have had. Give this man a promotion!"      /      "Professor Pappas did an excellent job teaching this class. Not only did he explain the content very well and answer any questions thoroughly, he went above and beyond in making us think critically about our futures unlike any Professor I've ever had. The knowledge, tips, and advice he has given us will be something we will all take into our futures and use to excel. Thank you Professor!"
title: Overview
toc: true
type: docs
weight: 1
---

## Flexibility

This feature can be used for publishing content such as:

* **Online courses**
* **Project or software documentation**
* **Tutorials**

The `courses` folder may be renamed. For example, we can rename it to `docs` for software/project documentation or `tutorials` for creating an online course.

## Delete tutorials

**To remove these pages, delete the `courses` folder and see below to delete the associated menu link.**

## Update site menu

After renaming or deleting the `courses` folder, you may wish to update any `[[main]]` menu links to it by editing your menu configuration at `config/_default/menus.toml`.

For example, if you delete this folder, you can remove the following from your menu configuration:

```toml
[[main]]
  name = "Courses"
  url = "courses/"
  weight = 50
```

Or, if you are creating a software documentation site, you can rename the `courses` folder to `docs` and update the associated *Courses* menu configuration to:

```toml
[[main]]
  name = "Docs"
  url = "docs/"
  weight = 50
```

## Update the docs menu

If you use the *docs* layout, note that the name of the menu in the front matter should be in the form `[menu.X]` where `X` is the folder name. Hence, if you rename the `courses/example/` folder, you should also rename the menu definitions in the front matter of files within `courses/example/` from `[menu.example]` to `[menu.<NewFolderName>]`.

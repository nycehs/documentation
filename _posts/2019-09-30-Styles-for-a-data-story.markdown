---
layout: post
title:  "Styles for a data story"
date:   2019-09-30 09:13:26 -0400
categories: styles

---
All "Closer look" data stories should run off of the same CSS file.

This file is accesible.css. It sets basic styles for basic, single-colum scrolling data stories. 

In particular, it features styles for the:
*Header that says "return to Data Stories"
*The title section with the large image and the special title and subtitle styles
*The column width
*The width of images and data visualizations that are wider than the standard column
*Header styles, text fonts, and link styles
*Footer that includes links

Some data stories also use story.css (stored in that data story's parent folder). This CSS file contains CSS that is specific to that story. I am working to deprecate that, making sure that each story runs off of a single, shared css file.
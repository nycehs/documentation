---
layout: post
title:  "Title images"
date:   2019-09-30 09:13:26 -0400
categories: Story CSS images HTML

---
All "Closer look" data stories have a title image.

This image should be stored in the same folder as the data story. For example, "Why asthma is a social justice issue" is /Closerlook/povasthma/index.html. The title image is stored in /povasthma. It is called /povasthma/title1.jpg.

Each title image should be called title1.jpg. 

Each story's Title1.jpg is referenced by in-line CSS in the story's main HTML file, which is /STORYNAME/index.html.

`<div class="titleslide" id="section0" style="background-image: url(title1.jpg) title="Insert an alt tag or image title here">`

You can change the name of the image file as long as you make sure to correctly reference it in the HTML file, but for ease of creating a new story by copying a previous one, simply calling each title image title1.jpg is a useful way to go. 

Some older stories reference this image via each story's custom css file, called story.css, but I am working to deprecate story.css so that all stories only use one shared css file - accessible.css.
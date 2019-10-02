---
layout: post
title:  "Title image text overlay"
date:   2019-10-2 09:13:26 -0400
categories: Story CSS images HTML

---
In a data story, you'll notice that the text starts in a way that overlaps the title image. This is intentional, to ensure that on small screens when the image loads full screen, that the `<h2>Main text title</h2>` loads visibly, enciting the reader to scroll down.

In order to do this, use `<div class="textwrap">` to enclose the first section of text - the part that comes before any later images or data visualizations. This class is set to shift upward so that it overlaps the previous component (in this case, the title image).

Later, use `<div class="textwrap2">`, which is not set to overlap. 


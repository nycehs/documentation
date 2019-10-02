---
layout: post
title:  "Inserting images"
date:   2019-10-2 10:13:26 -0400
categories: Story CSS images HTML Data

---
Images can be simply inserted by using the following code within `<div class="textwrap2">`:

~~~
<hr>
<span style="text-align:center; display:block;"><b>OPTIONAL IMAGE TITLE</b>
<img src="IMAGE URL" alt="Image Alt Text></span>
<hr>
~~~

Images can be set to expand on hover by including the following in css:

~~~
img {
    transition:transform 0.25s ease;
}

img:hover {
    -webkit-transform:scale(1.5);
    transform:scale(1.5);
}
~~~

Some stories have this in story.css, but it should be added to accessible.css.
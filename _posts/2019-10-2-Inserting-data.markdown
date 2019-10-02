---
layout: post
title:  "Inserting data"
date:   2019-10-2 10:13:26 -0400
categories: Story CSS images HTML Data

---
In a data story, you'll notice that data and images extend beyond text column, and have a grey background.

The column width is determined by `<div class="textwrap">` and `<div class="textwrap2">`. In order to insert data, close the previous textwrap div by using `</div>` and then start the code that we need to insert data:

~~~
<div class="datawrap">
<div class="datanarrow">
	Insert the iframe code for a data visualization or map here
	</div>
</div>
~~~
This sets up a wider column that's all grey, and inserts a narrower column within it for the data. It looks good to have data visualizations (or images) extend beyond the text column somewhat.


There are several different div classes that you can use instead of `<div class="datanarrow">`. These include `<div class="data">` (which is a little bit wider), `<div class="superwide">` (for things that should take up the full width of the pate), and `<div class="map">` (which, after some iterating, is the same as `<div class="datanarrow">`.

You can add new classes to accessible.css if you want to tweak the dimensions of a new div class for data inserts.
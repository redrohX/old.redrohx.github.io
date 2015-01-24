---
layout: post
title:  "Using Sass Maps to create a button library"
date:   2014-04-08
categories:
  - front-end
tags:
  - Sass maps
  - Button Library
excerpt: Last night I was browsing through Hugo Giraudel's excellent website, which is a great resource for a lot of uncommon Sass info...
image: /images/photos/europe-map.jpg

---
Last night I was browsing through Hugo Giraudel's excellent website,
which is a great resource for a lot of uncommon Sass info.
After reading [A Sass Component][1] in 10 minutes I hopped over to Codepen to put his ideas to paper and see what else I could come up with.

At some point I was looking at the Sass Maps example in Hugo's article, but since I was tired and 3.3 wasn't out yet anyway I would check it later.

The funny thing happened during the night, because I woke up with a message on Twitter that Sass 3.3 was released a few hours earlier. Imagine my joy!

That kind of motivated me to go back to Codepen and start working on a pen I was working on the night before: a [Sass button library][2] using the Maps feature.

The button library is based on the information found in Hugo's article, but I kind of extend upon it by adding a second map with button sizes.

I'm combining these Maps to create a library of different colors and sizes with just a little bit of code.

The amount of CSS it generates is pretty daunting, so if you're only going to use one or two of these buttons in your project it's completely overkill, but for a big project where you really need 16 buttons this is going to be pretty useful.

##Conclusion

The last month I've been doing research to see if Sass could be useful for projects at my current employer. I'm not the one that needs convincing, but there needs to be some hard evidence.
I think examples like these where I only write 57 lines of DRY code to create a small button library is proof enough that with Sass 3.3 we really can't ignore Sass anymore if you talk about front-end development.

<p data-height="268" data-theme-id="0" data-slug-hash="bvwtl" data-default-tab="result" class='codepen'>See the Pen <a href='http://codepen.io/redrohX/pen/bvwtl'>Sass Maps Button Library</a> by Niels van Rongen (<a href='http://codepen.io/redrohX'>@redrohX</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//codepen.io/assets/embed/ei.js"></script>

[1]: http://www.sitepoint.com/sass-component-10-minutes/
[2]: http://cdpn.io/bvwtl

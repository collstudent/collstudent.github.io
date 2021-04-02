---
layout: post
title:  Fixing Fonts
category: typo 
description: How I "fixed" a font I use.
---

I am quite picky when it comes to using fonts. For some time, I have been using the font **Sen** for all my work. It works well within my <img src="https://render.githubusercontent.com/render/math?math=\LaTeX"> documents - which I almost always use -  even for my Resume, Cover Letters, etc.


<p align="center">
<img align="center" src="https://raw.githubusercontent.com/collstudent/collstudent.github.io/master/assets/img/sen.png">
 </p>

  


However, as you might have observed, there is one problem!

It's the quotation marks (and similarly in the semicolon). It doesn't have "smart quotes". A similar issue is with the semicolon.

To fix this, I used the font editor *FontForge*, and another font whose characters seemed fine; I went with **Merriweather Sans**

<p align="center">
<img align="center" src="https://raw.githubusercontent.com/collstudent/collstudent.github.io/master/assets/img/mw.png">
 </p>


#### Attempt 1

I copied all uppercase/lowercase letters from *Sen* to *Merriweather Sans* in FontForge. However, it probably messed up the encoding and I got something weird!

<p align="center">
<img align="center" src="https://raw.githubusercontent.com/collstudent/collstudent.github.io/master/assets/img/mws.png">
 </p>


As you can see, the letters are indeed from *Sen* and the quotes are fancier. But the message is unreadable!

#### Attempt 2
I copied the comma, single/double quotes from *Merriweather Sans* to *Sen*. This worked! (I had to fix certain things using the *Transform* tool, but it wasn't that difficult)

<p align="center">
<img align="center" src="https://raw.githubusercontent.com/collstudent/collstudent.github.io/master/assets/img/senm.png">
 </p>

#### What's Next?
Well, I am still not happy with the **J**. It doesn't form a nice arc, and goes down the baseline. Maybe, in the future
, I will try to fix it. 

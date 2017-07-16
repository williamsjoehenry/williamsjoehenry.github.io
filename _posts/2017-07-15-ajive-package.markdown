---
layout: post
title:  "R and Python packages for AJIVE"
date:   2017-07-15
categories: software
---

I just released R and Python implementations of [Angle based Joint and Individual Variation Explained](https://arxiv.org/abs/1704.02060) (AJIVE). I recently started working on AJIVE for my thesis and releasing an open source package is one of my goals for my PhD. For the code see:

- [**ajive**](https://github.com/idc9/r_jive) (R)
- [**jive**](https://github.com/idc9/py_jive) (Python)

Both packages are currently a little rough (need more examples, more testing, cleaner code, fewer typos, etc), but they will improve with time and as I/other people use them. If you use one of these packages I encourage you to **send me critical feedback**. Right now the biggest areas in need of improvement are:

- More data analysis examples showing how AJIVE can be used.
- More testing to squash bugs I haven’t found.
- Better documentation -- both of the code and explaining the AJIVE procedure.

It feels wrong putting something out there that is not yet polished, but I figured it’s better to get something that works out there and improve it than to spend the rest of the summer perfecting it instead of writing my thesis (i.e. *don’t let the perfect be the enemy of the good*).

I learned a lot from building these packages. [This next post](/ajive-lessons.html) has some thoughts and advice about releasing software packages -- particularly for other graduate students. I will (hopefully soon) put up a few posts discussing how AJIVE works and showing some data analysis examples.

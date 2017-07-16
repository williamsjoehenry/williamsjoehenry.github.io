---
layout: post
title:  "R and Python packages for AJIVE and what I learned"
date:   2017-07-15
categories: software, AJIVE
---

I just released R and Python implementations of [Angle based Joint and Individual Variation Explained](https://arxiv.org/abs/1704.02060) (AJIVE). I recently started working on AJIVE for my thesis and releasing an open source package is one of my goals for my PhD. For the code see:

- [**ajive**](https://github.com/idc9/r_jive) (R)
- [**jive**](https://github.com/idc9/py_jive) (Python)

Both packages are currently a little rough (need more examples, more testing, cleaner code, fewer typos, etc), but they will improve with time and as I/other people use them. If you use one of these packages I encourage you to **send me critical feedback**. Right now the biggest areas in need of improvement are:

- More data analysis examples showing how AJIVE can be used.
- More testing to squash bugs I haven’t found.
- Better documentation -- both of the code and explaining the AJIVE procedure.

It feels wrong putting something out there that is not yet polished, but I figured it’s better to get something that works out there and improve it than to spend the rest of the summer perfecting it instead of writing my thesis (i.e. *don’t let the perfect be the enemy of the good*).

I learned a lot from building these packages. Below are some thoughts and advice about releasing software packages -- particularly for other graduate students.

# What I learned

There are some tradeoffs to consider:

- Academia does not seem to value software very much.
- There is a large time cost to develop software packages that could have been spent writing papers.

I think academia is starting to value software more than it used to[^1]. I would argue that, in many cases, releasing code is as important as writing a paper. Some of the benefits to you that come from releasing a software package include:

- Save future you time. Better code new = less headache in the future.
- Fame/glory/prestige for people using your work.
- Help other people solve their problems. If part of your rational for doing research/academia is helping to solve problems then good code might be as (or more) impactful as a paper.
- Software skills are highly valued in industry.
- You might learn new things out of necessity (e.g. computational linear algebra) and/or better understand your own research.


Programming is typically a small part of the statistics curriculum (and most other scientific disciplines); we don’t think of ourselves as software engineers even though many of us spend a lot of time writing code. Luckily there are many quality, open-source resources that show you how to write better code and release software. Without these resources (particularly the  [R Packages](http://r-pkgs.had.co.nz/) book) it would have taken me 1-2 orders of magnitude more time to build these packages[^2].


These resources are helpful for creating R/Python packages:

- Hadley Wickham’s [R Packages](http://r-pkgs.had.co.nz/)  book and [devtools](https://github.com/hadley/devtools) were incredibly helpful. If you plan on building an R package read this book.
- [This tutorial](http://python-packaging.readthedocs.io/en/latest/index.html) and [coockiecutter](https://github.com/audreyr/cookiecutter) give helpful templates and instructions to create a Python package.
- Tim Hopper’s [talk on releasing code](https://www.youtube.com/watch?v=uRul8QdYvqQ) gives a good high level overview of how/why to release code.
- [github](github.com)

These resources helped me become a better programmer:

- [Good Enough Practices in Scientific Computing](https://arxiv.org/pdf/1609.00037.pdf)
- [Some principles of good programming](http://www.artima.com/weblogs/viewpost.jsp?thread=331531)
- Jeff Leek’s book on [How to be a Modern Scientist](https://leanpub.com/modernscientist) and an uncountable number of [simplystatistics](https://simplystatistics.org/) posts.
- Unit testing made the packages a lot less buggy ([testthat](http://r-pkgs.had.co.nz/tests.html) for R and [unittest](https://github.com/ehmatthes/pcc/releases/download/v1.0.0/beginners_python_cheat_sheet_pcc_testing.pdf) for Python).
- Reading/borrowing from existing, quality bases including. I found the following helpful:
	- R: [ggplot2](https://github.com/tidyverse/ggplot2), [tidytext](https://github.com/juliasilge/tidytext). 
	- Python: [sklearn](https://github.com/scikit-learn/scikit-learn), [lightning](https://github.com/scikit-learn-contrib/lightning).

---
[^1]: For example, some [statistics postdoc](http://jtleek.com/jobs/) positions require (or highly encourage) applicants to have released an open source package.

[^2]: The time cost to build a package is obviously very context dependent (e.g. your experience, the complexity of the algorithm, etc). To give you one data point; these packages took me 1-2 weeks each and I have about 2 years of coding experience.
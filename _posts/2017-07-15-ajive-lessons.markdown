---
layout: post
title:  "Releasing software packages"
date:   2017-07-15
categories: software
---

[I recently released](/software/2017/07/15/ajive-package.html) my first [R](https://github.com/idc9/r_jive) and [Python](https://github.com/idc9/py_jive) packages. This post contains some thoughts and advice about releasing software packages – particularly for other graduate students.

First, there are some tradeoffs to consider:

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
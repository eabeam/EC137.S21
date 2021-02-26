---
title: "EC137"
author: "Emily Beam"
date: "2/16/2021"
output: html_document

---

# Lesson 1: Introduction to R





Things might get a bit tricky now! Don't worry. It will pay off. 

Why is this happening: 

	- Reproducibility is [important](http://www2.stat.duke.edu/courses/Fall17/sta112.01/slides/02-deck.html#5)
	- Things that were horrible in Excel are now faster and more pleasant
	- We can make some really pretty things using `ggplot` and friends.

What is version control, and why do we care?

What is R vs RStudio?)[)

*What if I'm lost? * Message the Teams channel. Think of it as an ongoing conversation



Also, have you identified who in your small group has worked w/ R? Now might be a good time to get to know them better! 



Assignment: 

- Watch [this short video](video) I made to introduce you to R 
- Read the explanation below
- Download R and R studio
- Complete the following R tutorials 

Download R Studio 

### Instructions

1. First, we need to actually get you some [R](https://www.r-project.org/). You can download R from [CRAN](https://cran.r-project.org/mirrors.html). You'll see a whole host of "mirrors" - pick any one you like. 

2. Then, you need to download RStudio. You can either get the standard version (RStudio Desktop) [here](https://rstudio.com/products/rstudio/download/preview/), or you can grab a ["preview" version](https://rstudio.com/products/rstudio/download/preview/), which has fun new updates. I recommend preview version, but it's your call.

3. Once you have both installed, open RStudio. You know things are good if you see something that looks like a emptier, sadder version of [this.](https://rstudio.com/wp-content/uploads/2014/04/rstudio-workbench.png)

4. Now, the test to see if things are working. 

   a. Put your cursor in the pane labelled **Console**

   b. Type the following: `x <- 2*2` and press enter/return. You've made an object! it's name is `x` and it's equal to `2*2`

   c. Type the following: `x`  and press enter/return. This prints the object. Do you see the number 4? Success!

   

   What if you are stuck? *Head to Teams!*

   

   ## Packages 

   R itself can do all sorts of neat statistical things. But, the bulk of its functionality is not included in the base installation. Rather, we need packages. 

   Packages are a set of programs that live on your computer. You only need to install them once. We need three important packages: 

   - [dplyr](https://cran.r-project.org/package=dplyr)
   - [ggplot2](https://ggplot2.tidyverse.org/)
   - [tidyr](https://tidyr.tidyverse.org/)

   We can easily install them using the `install.packages` command. Type the following into your command window and press enter 

``` install.packages("dplyr", dependencies = TRUE)
install.packages("dplyr", dependencies = TRUE)
```

Notice that there are two parts: (1) `"dplyr"`  - the name of the package in double-quotation marks; and (2) `dependencies = TRUE` - which tells R to make sure to download any packages that `dplyr` needs to run properly. 



**Install `dplyr`**, **`ggplot2`**, and **`tidyr`**





For those of you with some R experience, you may be familiar and comfortable uniting the power of R with RMarkdown and Git. I'm happy for you to do either or both. From my own experience I'm great at RMarkdown and "advanced beginner" at Git. 



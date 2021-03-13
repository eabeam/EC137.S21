---
title: "Lesson 1: Introduction to R"
author: "Emily Beam"

output: html_document

---

# Lesson 1: Introduction to R

## What you'll learn: 

**Before class (on your own)**

1. Download and install R and RStudio.
2. Complete a tutorial
3. Make sure you can run commands in the command window sucessfully

**In class**

1. RStudio walkthrough
2. General principles of R
3. Using RMarkdown

## Lesson

Now we're beginning our R unit. As with Excel, there is *wide variation* in our baseline background with R, perhaps even more so! We will take **two weeks** to set aside all policy applications and just think about R. 

#### *What does this mean?* 

**Never used R:** This is where I am teaching from. If I get too jazzed and you need extra clarification/help, please each out to group mates who have used R and will be able to explain things in a new/different way. If they are stumped, reach out to me! 

**Used R but rusty:** This should be just right for you, but there will be some review. Enjoy the easy ride! 

**Confident R user**: There will be a *lot* of review. I will occasionally provide alternative activities you can do instead of the assigned ones if you want to push yourself. It is up to you which you do (and you can jump back and forth, depending on your workload). 

Things might get a bit tricky now! Don't worry. It will pay off. 

**Why is this happening:** 

- Reproducibility is [important](http://www2.stat.duke.edu/courses/Fall17/sta112.01/slides/02-deck.html#5)
- Things that were horrible in Excel are now faster and more pleasant
- We can make some really pretty things using `ggplot` and friends.

**What if I'm lost?**

- Message the Teams channel. Think of it as an ongoing conversation
- Also, have you identified who in your small group has worked w/ R? This is good for everyone to know!

For those of you with some R experience, you may be familiar and comfortable uniting the power of R with RMarkdown and Git. I'm happy for you to do either or both. In terms of the support I an provide, I'm quite experienced with RMarkdown and "decently competent beginner" at Git. 

## Installing R

You can download R from [CRAN](https://cran.r-project.org/). Select your operating system. 

**Windows users**: Select `base`, and then download and install R

**Mac users**: Download and install R-4.04.pkg

If you get an error message, then you should hold down the `control` key while clicking the package, then select "open" (still holding the key), and once you see a warning message, select "open."

## Install RStudio

1. Then, you need to download RStudio. You can either get the standard version (RStudio Desktop) [here](https://rstudio.com/products/rstudio/download/preview/), or you can grab a ["preview" version](https://rstudio.com/products/rstudio/download/preview/), which has fun new updates. I recommend preview version, but it's your call.

2. Once you have both installed, open RStudio. You know things are good if you see something that looks like a emptier, sadder version of [this.](https://rstudio.com/wp-content/uploads/2014/04/rstudio-workbench.png)

3. Now, the test to see if things are working. 

   a. Put your cursor in the pane labelled **Console**

   b. Type the following: `x <- 2*2` and press enter/return. You've made an **object**! it's name is `x` and it's equal to `2*2`

   c. Type the following: `x`  and press enter/return. This prints the object. Do you see the number 4? Success!

   

   What if you are stuck? *Head to Teams!*

   

## Packages 

R itself can do all sorts of neat statistical things. But, the bulk of its functionality is not included in the base installation. Rather, we need packages. 

Packages are a set of programs that live on your computer. You only need to install them once. We will need three important packages: 

- [dplyr](https://cran.r-project.org/package=dplyr)
- [ggplot2](https://ggplot2.tidyverse.org/)
- [tidyr](https://tidyr.tidyverse.org/)

We can easily install them using the `install.packages` command. Type the following into your command window and press enter 

```R
install.packages("dplyr", dependencies = TRUE)
```

Notice that there are two parts: 

1.  `"dplyr"`  - the name of the package in double-quotation marks; and 
2.  `dependencies = TRUE` - which tells R to make sure to download any packages that `dplyr` needs to run properly. This is optional.



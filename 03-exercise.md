---
title: "Exercise 3"
author: "Emily Beam"

output: html_document


---

# Exercise 3

**Due 28 March @ 11:59pm**

[TOC]

**You can work individually or in pairs.** If you work in pairs, you may submit one assignment for the two of you. It is, of course fine if you talk with and work with more than one other person, but I'm capping it as two submitters assignment so I don't end up grading two assignments total.





## Getting started

The New York City Department of Buildings (DOB) maintains a list of  construction sites that have been categorized as “essential” during the  city’s shelter-in-place pandemic order. They’ve provided [an interactive map here](https://www1.nyc.gov/assets/buildings/html/essential-active-construction.html) where you can see the different projects. There’s also a link there to download the complete dataset.

For this exercise, you’re going to use this data to visualize the amounts or proportions of different types of essential projects in the  five boroughs of New York City (Brooklyn, Manhattan, the Bronx, Queens,  and Staten Island).

Either create a new project for this exercise only, or make a project for all your work in this class.

You’ll need to download one CSV file and put it somewhere on your computer or upload it to RStudio.cloud—preferably in a folder named `data` in your project folder. You can download the data from [the DOB’s map](https://www1.nyc.gov/assets/buildings/html/essential-active-construction.html), or use this link to get it directly:

- [`EssentialConstruction.csv`](EssentialConstruction.csv)

To help you, I’ve created a skeleton R Markdown file with a template  for this exercise, along with some code to help you clean and summarize  the data. Download that here and include it in your project:

- [`03_exercise_template.Rmd`](03_exercise_template)

In the end, the structure of your project directory should look something like this:

```
your-project-name\
  03_exercise.Rmd
  your-project-name.Rproj
  data\
    EssentialConstruction.csv
```

To check that you put everything in the right places, you can instead download and unzip this file, which contains everything in the correct structure:

- [`03_exercise.zip`](03_exercise.zip)



### Part 1: Essential pandemic construction

Make the following plots:

- Show the count *and* proportion of approved projects by borough using a **bar chart**
- Show the count *or* proportion of approved projects by category using a **lollipop chart**
- Show the proportion of approved projects by borough *and* category simultaneously using a **heatmap**

*The examples from 08-01 and 08-02 will be extremely helpful!*

You’ll need to insert your own code chunks where needed. Rather than  typing them by hand (that’s tedious and you might miscount the number of backticks!), use the “Insert” button at the top of the editing window,  or type ctrl + alt + i on Windows, or ⌘ + ⌥ + i on macOS.

### Part 2: Reflection

At the bottom of your document, answer the following two questions: 

- Briefly explain what each plot shows
- What design decisions did you make, and why?
- What challenges did you encounter or questions were you unable to answer? 
- What resources did you use to soldier on? 



### Part 3: Turning everything in

When you’re all done, click on the “Knit” button at the top of the  editing window and create an HTML or Word version (or PDF if you’ve [installed **tinytex**](https://datavizm20.classes.andrewheiss.com/resource/install/#install-tinytex)) of your document. Upload that file to Blackboard.

There will be a quick "quiz" on BB. Again, if you're working with a buddy, one quiz can apply to both people. 



## Advanced Users

Upon reflection, I think most advanced users will still get something out of this assignment. Specifically, I'd encourage you experiment with color schemes and labels, as described above. 

However, if you'd like a different sort of challenge, you can complete an alternate assignment: create a demo/tutorial on a feature that we won't be able to directly explore in class: 

1. Select a prodedure/pacakge [from the list](https://docs.google.com/spreadsheets/d/1pAHKMGHwS-Z8dgQXDTgzcg65w_-F08GAkyo5mM4PC3Q/edit?usp=sharing) and sign up to "claim" it. (I'm also open to other suggestions if you e-mail me)
2. Create a simple working demonstration using data that might be relevant to our class. I would recommend [`blscrapeR`](https://github.com/keberwein/blscrapeR); [`wdi`](https://cran.r-project.org/web/packages/WDI/WDI.pdf), or our TidyTuesday data. (This is not a requirement)
   1. I recommend using the [`reprex()`](https://www.tidyverse.org/help/#reprex) package to ensure your example is reproducible
3. Create a short video in which you "demo" the package, providing clear explanation to relatively new users about how to utilize the package. 
4. Upload the demonstration code, output file (pdf/html), and link to the video. I'll share these on blackboard as resources for your classmates!

If you go this route...

- You can (as always!) help each other, but here it is **one video and one topic per person**.
- You can skip the BB quiz for Exercise 03
- You don't need to notify me in advance what you pick.



**Possibilities:** 

- Create a choloropleth map using ggplot2 
- Add [annotations](https://ggplot2.tidyverse.org/reference/annotate.html) to a plot using `annotate()`
- Merge files using `joinby()` (discuss inner, left, right, full)
- How to get data out of `blscrapeR`
- How to get data out of `wdi`
- How to work with [`lubridate()`](https://lubridate.tidyverse.org/articles/lubridate.html)


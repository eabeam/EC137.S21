# [Unit 2] Pre-Class Activities



[TOC]



## PC March 16 - Introduction to R (07-01)

The purpose of this pre-class activitiy is to get you set up for us to introduce R in class. See below if you're an advanced user.



### Assignment

1. Install R

   You can download R from [CRAN](https://cran.r-project.org/). Select your operating system. 

   **Windows users**: Select `base`, and then download and install R

   **Mac users**: Download and install R-4.04.pkg

   If you get an error message, then you should hold down the `control` key while clicking the package, then select "open" (still holding the key), and once you see a warning message, select "open."

3. Install R Studio. You can either get the standard version (RStudio Desktop) [here](https://rstudio.com/products/rstudio/download/preview/), or you can grab a ["preview" version](https://rstudio.com/products/rstudio/download/preview/), which has fun new updates. I recommend preview version, but it's your call.

4. Complete [Programming Basics](https://rstudio.cloud/learn/primers/1.2) tutorial (*Note: you will need to create a free RStudio Cloud account*). In terms of time budgeting, note that this will involve you watching 7 videos that are 1-2 minutes long. There will also be short activities you can do, in which you type into boxes and click "run code" to test it. You should do these too!

5. Open RStudio on your computer. You know things are good if you see something that looks like a emptier, sadder version of [this.](https://rstudio.com/wp-content/uploads/2014/04/rstudio-workbench.png)

6. Type the following code in your Console window and press Enter:  `sqrt(pi)`. Look, you calculated $\sqrt{\pi}$!

6. Install the tidyverse! Type the following code in your Console window and press Enter: 

   ```R
   install.packages("tidyverse")
   ```

   It incldues fun friends like `dplyr` (pronounced "dee-plier") and more!

   

7. Tell R to use `dplyr`. Type the following code in your Console window and press Enter: 

   ```R
   library(dplyr)
   ```

8. Make sure your computer can do all the things: Type or copy-paste the following code in your Console window and press Enter:  

```R
starwars %>% 
  filter(species == "Droid")
```

​		What is IG-88's height, mass, and homeworld? 

![IG-88's profile](images/ig88.png)



#### Advanced user?

 Most of this will not be necessary. You should still answer the prompts, which will require you to do parts (7) and (8) of the [assignment](#Assignment).

The [R Introduction](R_0601_intro.html) page contains instructions on installing R and R Studio, plus some general background.

### Submit

Submit on Blackboard the answers to the following questions (in our pre-class assignments)

1. Tell me a bit about your comfort level and experience with R. What would be useful for me to know?
2. If you haven't used R before, what challenges did you encounter going through the following steps? What questions do you have? 
3. What is IG-88's height, mass, and homeworld? 



---

## PC March 18 - Introduction to `dplyr` (07-02)



### Assignment

Complete the following 3 primers:

1. [Data visualization basics](https://rstudio.cloud/learn/primers/1.1)
2. [Working with tibbles](https://rstudio.cloud/learn/primers/2.1)
3. [Isolating data with `dplyr`](https://rstudio.cloud/learn/primers/2.2)

You'll notice that you can work through examples in the tutorial, run your code, and compare against the solutions. I strongly recommend that you copy and paste your code into a R script or R markdown document as you go, which will give you a record of what you've done. You'll also need to bring in some answers in order to generate your PC document (below).

The remaining instructions are available [here](R_0702_template.html). You'll want to download the following [template](R_0702_template.Rmd) and open it in RStudio.



#### Advanced user? 

If you are already comfortable with RMarkdown, `dplyr`, and the rudiments of `ggplot`, then don't do the assignment. Instead, do the following: 

1. Install the `babynames` package. 
2. Pick a movie or TV show that has had very specific names. If you're stuck, you could think about Dallas, 90210, Game of Thrones, basically any popular Disney movie, any movie from the Star Wars franchise, etc. 
3. Make a plot of the rise (and fall?) of a set of names (as a share of all baby names of that gender) from that show over time. **OR**, make a different sort of graph (which Disney movie princess has affected a larger share of names?)! Bring in a new theme using the `ggthemes` package if you'd like.
4. Put your code and output in a .Rmd file and knit to PDF/word/html. Upload that instead.

### Submit

Your output should be a Word/PDF/html (pick whichever) that you created by knitting from the template that you edited. Note that if you try to upload a html file on to Blackboard, you will need to compress/zip it first. 



## PC March 23 - Introduction to {`ggplot2`}

### Assignment

Complete these four primers:

1. [Derive information with `dplyr`](https://rstudio.cloud/learn/primers/2.3): practice w/ pipes and other key commands: `summarize()`, `mutate()`, and `group_by()`
2. (Optional) [Exploratory data analysis](https://rstudio.cloud/learn/primers/3.1) : this one is fairly short (no coding), but it's a good review about how to think about exploring data, categorical and continuous variables, and what types of visualizations are useful for what types of exploration. It's okay with me if you skip this one if you already feel confident with these concepts. 
3. [Bar charts](https://rstudio.cloud/learn/primers/3.2)
4. [Histograms](https://rstudio.cloud/learn/primers/3.3)

The remaining instructions are available here: [R_0801_pc_template.html](R_0801_pc_template.html) You'll want to download the following template and open it in RStudio: [R_0801_pc_template.Rmd](R_0801_pc_template.Rmd)

#### Advanced user? 

If you are already comfortable with `dplyr`, and these `ggplot` basics, then don't do the assignment. Instead,  let's do a quick TidyTuesday assignment! 

Because we're going to be tackling inequality (or rather, examining inequality) in a week or two, I'll ask you to make one neat graph based on the 02-09-2021 TidyTuesday - wealth and income! 

1. [Instructions](https://github.com/rfordatascience/tidytuesday/blob/master/data/2021/2021-02-09/readme.md) to install and load the package and data. You can either download the entire package, or you can manually pick just one or a handful of files. 
2. Browse through the data and select one (or more, if you feel like merging) files to work with.
3. Create a **bar chart or histogram** (or a related variant) that is of interest to you! 
4. Upload a pdf/ zipped html file with your results.

The internet is full of inspiration, as participants post their results and code on Twitter with [#tidytuesday](https://mobile.twitter.com/search?q=tidytuesday%20until%3A2021-02-15%20%20since%3A2021-02-09&src=typed_query). You'll want to go back to posts around [February 09-15](https://mobile.twitter.com/search?q=tidytuesday%20until%3A2021-02-15%20%20since%3A2021-02-09&src=typed_query) ( :point_left:  :point_left: embedded in the link). You can start from scratch of build off what other folks have done. 



### Submit

Finally, knit this document to Word, html, or PDF and upload into Blackboard. 

- PDF: If you want to use PDF but are getting an error, install the `tinytex` package. This is a two-step process. Andrew Heiss provides the [clearest explanation.](https://datavizm20.classes.andrewheiss.com/resource/install/)
- html: BB will only let you upload a html file if you compress it first! :cry:

*Note:* If you get a weird error message about `Error in contrib.url(repos,"source")...` comment out the two lines that install your packages.





## PC March 30 - `ggplot2` - the return!

### Assignment

Complete the following tutorials: 

1. (Optional) [Box plots and counts](https://rstudio.cloud/learn/primers/3.4): Coverage of additional graph types that are handy but not critical
2. [Scatterplots](https://rstudio.cloud/learn/primers/3.5)
3. [Line plots](https://rstudio.cloud/learn/primers/3.6)
4. [Customize plots](https://rstudio.cloud/learn/primers/3.8)

Then, download and work through the pre-class template here: [R_0901_pc_template.Rmd](R_0901_pc_template.Rmd). 

You can find the html version as well: [R_0901_pc_template.html](R_0901_pc_template.html).

#### Advanced user? 

If you are already comfortable with `ggplot` , then don't do the assignment. Instead, let's revisit our TidyTuesday assignment ... for Thursday. 

That said, you. may still want a quick refresher with the final `ggplot` primer: [Customize plots](https://rstudio.cloud/learn/primers/3.8) - there is good practice with labels, themes, scales (with `scale_color_brewer` and `scale_fill_brewer`), and legends. 

Dive back into the 02-02-2021 Tidy Tuesday on wealth and income over time.! 

1. [Instructions](https://github.com/rfordatascience/tidytuesday/blob/master/data/2021/2021-02-09/readme.md) to install and load the package and data. You can either download the entire package, or you can manually pick just one or a handful of files. 
2. Browse through the data and select one (or more, if you feel like merging) files to work with.
3. Create a **scatter plot or line plot** (or a related variant) that is of interest to you! 
4. Make it pretty with lables, themes, colors.
5. Upload a pdf/ zipped html file with your results.

The internet is full of inspiration, as participants post their results and code on Twitter with [#tidytuesday](https://mobile.twitter.com/search?q=tidytuesday%20until%3A2021-02-15%20%20since%3A2021-02-09&src=typed_query). You'll want to go back to posts around [February 09-15](https://mobile.twitter.com/search?q=tidytuesday%20until%3A2021-02-15%20%20since%3A2021-02-09&src=typed_query) ( :point_left:  :point_left: embedded in the link). You can start from scratch of build off what other folks have done. 

### Submit

Finally, knit this document to Word, html, or PDF and upload into Blackboard. 

- PDF: If you want to use PDF but are getting an error, install the `tinytex` package. This is a two-step process. Andrew Heiss provides the [clearest explanation.](https://datavizm20.classes.andrewheiss.com/resource/install/)
- html: BB will only let you upload a html file if you compress it first! :cry:

*Note:* If you get a weird error message about `Error in contrib.url(repos,"source")...` comment out the two lines that install your packages.




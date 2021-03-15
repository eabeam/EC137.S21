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

All instructions are available [here](R_0702_template.html). You'll want to download the following [template](R_0702_template.Rmd) and open it in RStudio.





#### Advanced user? 

If you are already comfortable with RMarkdown, `dplyr`, and the rudiments of `ggplot`, then don't do the assignment. Instead, do the following: 

1. Install the `babynames` package. 
2. Pick a movie or TV show that has had very specific names. If you're stuck, you could think about Dallas, 90210, Game of Thrones, basically any popular Disney movie, any movie from the Star Wars franchise, etc. 
3. Make a plot of the rise (and fall?) of a set of names (as a share of all baby names of that gender) from that show over time. **OR**, make a different sort of graph (which Disney movie princess has affected a larger share of names?)! Bring in a new theme using the `ggthemes` package if you'd like.
4. Put your code and output in a .Rmd file and knit to PDF/word/html. Upload that instead.



### Submit

Your output should be a Word/PDF/html (pick whichever) that you created by knitting from the template that you edited. 
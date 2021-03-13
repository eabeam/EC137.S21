# [Unit 2] Pre-Class Activities



[TOC]



## PC March 16 - Introduction to R (07-01)

The purpose of this pre-class activitiy is to get you set up for us to introduce R in class.

Previous R user? Most of this will not be necessary. You should still answer the prompts, which will require you to do parts (7) and (8) of the [assignment](#Assignment).

The [R Introduction](R_0601_intro.html) page contains instructions on installing R and R Studio, plus some general background.

### Assignment

1. [Install R](R_0601_intro.html/#Install-R)

   You can download R from [CRAN](https://cran.r-project.org/). Select your operating system. 

   **Windows users**: Select `base`, and then download and install R

   **Mac users**: Download and install R-4.04.pkg

   If you get an error message, then you should hold down the `control` key while clicking the package, then select "open" (still holding the key), and once you see a warning message, select "open."

3. [Install RStudio](R_0601_intro.html/#Install-RStudio)

4. Complete [Programming Basics](https://rstudio.cloud/learn/primers/1.2) tutorial (*Note: you will need to create a free RStudio Cloud account*). In terms of time budgeting, note that this will involve you watching 7 videos that are 1-2 minutes long. There will also be short activities you can do, in which you type into boxes and click "run code" to test it. You should do these too!

5. Open RStudio on your computer.

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

![IG-88's profile](/Users/emilybeam/Dropbox/EC137.S21/?u=https%3A%2F%2Fstatic.comicvine.com%2Fuploads%2Foriginal%2F11135%2F111355667%2F6486631-100029-ig88-990x600.jpg&f=1&nofb=1.png)

### Submit

Submit on Blackboard the answers to the following questions (in our pre-class assignments)

1. Tell me a bit about your comfort level and experience with R. What would be useful for me to know?
2. If you haven't used R before, what challenges did you encounter going through the following steps? What questions do you have? 
3. What is IG-88's height, mass, and homeworld? 


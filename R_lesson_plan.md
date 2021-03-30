# Lesson Plan 

## 07.01 Intro

### Before class 

Install R, install RStudio

Complete [Programming Basics](https://rstudio.cloud/learn/primers/1.2) tutorial

- Functions

- Arguments

- Objects

- Vectors

- Types

- Lists

- Packages

  ### During class

1. Overview of unit
2. Introduction to R - walk through interface 
3. Installing packages, library 
4. General principles
5. Setting up and running R Markdown 
6. In small groups - make a basic RMarkdown file 



## 07.02 Tidyverse

Before class

1. [Data visualization basics](https://rstudio.cloud/learn/primers/1.1)
2. [Working with tibbles](https://rstudio.cloud/learn/primers/2.1)
3. [Isolating data with `dplyr`](https://rstudio.cloud/learn/primers/2.2)



Deliver this lesson: https://datavizm20.classes.andrewheiss.com/lesson/04-lesson/

Turn the activities into small group activities 



## 08.01 Graphics 

Deliver this lesson https://datavizm20.classes.andrewheiss.com/example/04-example/



## 08.02 Graphics II 



## Exercise 03 

Mini-assignment https://	.classes.andrewheiss.com/assignment/03-exercise/

Mini-assignment https://datavizm20.classes.andrewheiss.com/assignment/04-exercise/

https://datavizm20.classes.andrewheiss.com/assignment/08-exercise/#task-3-slopegraphs-1 <-- look its our BLS slope graphs. OMG this is faster. 

*Advanced:* Select one plot from part 2. Use ggthemes to make it the UGLIEST PLOT IN THE WORLD. Select another plot from part 3. Use ggthemes to make it the BEST PLOT IN THE WORLD 



## Advanced Users

In lieu of the above assignment, you can do the following: 

Sign up for a procedure/package here. 

Create a simple working demonstration of the package or produre 

Create a short video in which you "demo" the package, providing clear explanation to relatively new users about how to utilize the package. 

Upload the demonstration code, output file (pdf/html), and link to the video. I'll share these on blackboard as resources for your classmates!

Ideally, you would use data that might be relevant to our class - I would recommend [`blscrapeR`](https://github.com/keberwein/blscrapeR); [`wdi`](https://cran.r-project.org/web/packages/WDI/WDI.pdf), or our TidyTuesday data 

Possibilities: 

- Create a choloropleth map using ggplot2 
- Add [annotations](https://ggplot2.tidyverse.org/reference/annotate.html) to a plot using `annotate()`
- 
- 
- 

## 09.01 Graphics (*rescheduled 08-02*)

1. Cover things that are confusing people: 

   1. `mutate()`
   2. `group_by()`
   3. `ungroup()`

   https://datavizm20.classes.andrewheiss.com/content/05-content/#slides

2. Disuss aesthetics with `ggplot` and themes: 

   1. Reviewing the standard `ggthemes`
   2. Looking at custom theme packages others have used 
   3. Creating and editing your own theme elements
      1. Custom colors
      2. Custom fonts
   4. Saving and exporting plots with `ggsave`

3. Importing data 

   1. csv files

   2. > ```
      > library(readr)
      > 
      > data2 <- read_csv("C:\\Users\\Bob\\Desktop\\data.csv")
      > 
      > 
      > library(data.table)
      > 
      > data3 <- fread("C:\\Users\\Bob\\Desktop\\data.csv")
      > ```

   3. excel files 

   4. working with packages to get data 

   5. 

## 08.02 Policy brief



## 09.01 Inequality

Exercise 4: https://www.core-econ.org/doing-economics/book/text/05-03.html#part-52-measuring-other-kinds-of-inequality Just do this entire thing (EB write it out more specifically )

https://datavizm20.classes.andrewheiss.com/example/08-example/ -- using WDI to analyze things - we coudl pick inequality data 

Exercise 5: https://www.core-econ.org/doing-economics/book/text/12-03.html This one 

Later on: Plotting with time: https://datavizm20.classes.andrewheiss.com/example/11-example/



## R in the wild: 

1. Importing csv files 
2. [Reshape data](https://rstudio.cloud/learn/primers/4.1)



## 11 Intergenerational mobility 

https://opportunityinsights.org/course/

Find yourself


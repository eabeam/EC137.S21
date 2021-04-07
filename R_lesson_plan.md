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





Week 10: Next time, use [this](https://uvmoffice-my.sharepoint.com/:p:/g/personal/ebeam_uvm_edu/EZU8QhALi6BBjOjzvGJnTGIBu7lmjEJEOIE2WwGEU54ilg?e=ILT3Pm)

## Week 11 - Inequality

**Exercise 04 due at the end of the week!**

### {11-01} 04/13 Impact of policy on inequality

| ---                   | ---      |                                                              |
| --------------------- | -------- | ------------------------------------------------------------ |
| **Pre-class**         | Read     |                                                              |
|                       | Complete | Complete 11-01 pre-class activity on Blackboard              |
| **Lesson**            |          | [Lecture 3 Moving to Opportuinty](https://uvmoffice-my.sharepoint.com/:p:/g/personal/ebeam_uvm_edu/EVBP4vsS_RpDgWURDwbY6RcBvY_qYvXkxd13ue3lkBvlog?e=mF8xQO) (Chetty) |
| **In-class activity** |          |                                                              |



In another life: 

D. Hamilton and W. Darity, Jr. (2010). Can ‘Baby Bonds’ Eliminate the Racial Wealth Gap in Putative Post-Racial America? *Review of Black Political Economy*, 37(3,4):207-216.

### ~~{11-02} 04/15 No class - respite day~~

## Week 12 - Capstone

### {12-01} 04/20 Project showcase

Submit your draft slides on Blackboard before class

### {12-02} 04/22 Policy writing workshop

We'll cover the art of policy writing to gear up for the final capstone



# Unit 3: Putting it all together

## Week 13 - Higher education

**Exercise 05 due at the end of the week!**

### {13-01} 04/27 Returns to education



| ---                   | ---      |                                                              |
| --------------------- | -------- | ------------------------------------------------------------ |
| **Pre-class**         | Read     | **(p10)** Webber, Douglas. [“Is the Return to Education the Same for Everybody?](https://wol.iza.org/articles/is-the-return-to-education-the-same-for-everybody/long)” *IZA World of Labor*, October 1, 2014. *Read the "long"* version! |
|                       | Complete | Answer reading response questions on Blackboard              |
| **Lesson**            |          | [Lecture 7 Education 2 (Chetty)](https://uvmoffice-my.sharepoint.com/:p:/g/personal/ebeam_uvm_edu/EY7dRwf24B1DnRy_yaf4W7YBNJX0t9XTQXxiMI6Pwrf0Yw?e=AK2q07) *Causal impact of education* |
| **In-class activity** |          |                                                              |



### {13-02} 04/29 Education and income mobility

[Lecture 6, education 1](https://uvmoffice-my.sharepoint.com/:p:/g/personal/ebeam_uvm_edu/EQ2kDCeFADVNoPa4Xj4QlQ0BMHSyfEyZ6kt3QmB98rF9Tg?e=kjuJdV) (Chetty) *Education and income mobility*



| ---                   | ---      |                                                              |
| --------------------- | -------- | ------------------------------------------------------------ |
| **Pre-class**         | Read     | Carey, K. ["What about tackling the causes of student debt?](https://www.nytimes.com/2020/11/18/upshot/student-debt-forgiveness-biden.html) *The New York Times.* 18 November 2020. |
|                       |          | **(8p)** Fry, R. ["The changing profile of student borrowers."](https://www.pewresearch.org/social-trends/2014/10/07/the-changing-profile-of-student-borrowers/) Pew Research Center. 07 Oct 2014. |
|                       |          | **(3p)** Dynarski, S. ["Student Debt"](https://inequality.stanford.edu/sites/default/files/Pathways_SOTU_2019_StudentDebt.pdf) *The Poverty and Inequality Report 2019* |
|                       | Complete | Download the data from the chart in the NYT article by clicking on the source (it's a `.csv` file, so you may need to right click --> save link as). Using R or Excel, recreate the chart but adjust it for inflation. Make it pretty |
| **Lesson**            |          |                                                              |
| **In-class activity** |          |                                                              |





## Week 14 - Student debt

### {14-01} 05/04 Impacts of student debt



| ---                   | ---                 |                                                              |
| --------------------- | ------------------- | ------------------------------------------------------------ |
| **Pre-class**         | Read                | Black, Sandra, Amy Filipek, Jason Furman, Laura Giuliano, and Ayushi Narayan. “Student Loans and College Quality: Effects on Borrowers and the Economy.” *VoxEU.Org* (blog), August 4, 2016. https://voxeu.org/article/student-loans-and-college-quality-effects-borrowers-and-economy. |
|                       | Complete            |                                                              |
|                       | *Optional readings* | Elliot, W. and Nam, I. ["Is student debt jeopardizing the short-term financial health of US households?"](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.401.2486&rep=rep1&type=pdf) *Federal Reserve Bank of St Louis Review.* September/October 2013. |
| **Lesson**            |                     |                                                              |
| **In-class activity** |                     |                                                              |



### 

### {14-02} 05/06 Student debt reform



| ---                   | ---      |                                                              |
| --------------------- | -------- | ------------------------------------------------------------ |
| **Pre-class**         | Read     | **(10p)** Chapman**, Bruce. [“Income Contingent Loans in Higher Education Financing.”](https://wol.iza.org/articles/income-contingent-loans-in-higher-education-financing/long) *IZA World of Labor*, February 1, 2016. *(read the "long" version!)* |
|                       | Complete |                                                              |
| **Lesson**            |          |                                                              |
| **In-class activity** |          |                                                              |



### 

## Week 15 - Conclusion

### {15-01} 05/11 Project showcase 

Our lass class! :sob:



| ---                   | ---  |                                 |
| --------------------- | ---- | ------------------------------- |
| **Pre-class**         |      | Prepare your policy brief draft |
| **Lesson**            |      |                                 |
| **In-class activity** |      |                                 |


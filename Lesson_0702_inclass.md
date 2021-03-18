---
title: "Lesson 07-02: In-class assignment"
author: "NAME"
date: "3/18/2021"
output: html_document

---

*These lessons draw heavily from the excellent book, [R for Data Science](https://r4ds.had.co.nz/workflow-basics.html)*

## In-Class Assignment

In your groups, complete these exercises:

1. Why does this code not work? Fix it! (look extremely closely!)

```
my_variable <- 10
my_varıable
```

2. Fix this code so it runs. There are three errors!

```
library(tidyverse)

ggplot(dota = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy))

fliter(mpg, cyl = 8)
filter(diamond, carat > 3)
```

3. Press alt-shift-K. What happens? Can you find it using the drop-down menu?



4. Run this block of code to load the `nycflights` package. You will also need to load tidyverse if you didn't run the previous block of code

   ```
   library(nycflights)
   ```

   


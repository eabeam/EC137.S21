---
title: "Lesson 07-02: Introduction to `dplyr`"
author: "Emily Beam"
date: "3/18/2021"
output: html_document
---

*These lessons draw heavily from the excellent book, [R for Data Science](https://r4ds.had.co.nz/workflow-basics.html)*



[TOC]



## Objectives

Become comfortable with the following concepts 

| --   | --   | --   |
| ---- | ---- | ---- |
|      |      |      |

Become comfortable with the following commands from `dplyr`

- Extract rows/cases with `filter()`
- Extract columns/variables with `select()`
- Arrange/sort rows with `arrange()`
- Make new columns/variables with `mutate()`
- Make group summaries with `group_by %>% summarize()`

Every **dplyr** verb follows the same pattern. The first argument is always a data frame, and the function always returns a data frame:

```r
VERB(DATA_TO_TRANSFORM, STUFF_IT_DOES)
```

## Recap

#### Basics

We can use R as a calculator. You can enter all sort of things in the console.

```r
1 / 200 * 30
#> [1] 0.15
(59 + 73 + 2) / 3
#> [1] 44.66667
sin(pi / 2)
#> [1] 1

```

You can create new objects with `<-`. This is an *assignment statement* because it assigns something to an object. 

```
object_name <- value
```

Object names must start with a letter, and can only contain letters, numbers, `_` and `.`. It is a good idea to use words that are descriptive. Personally, i like **snake_case** because when you double click on it, you select the entire object (rather than **this-way**) 

```
i_use_snake_case
otherPeopleUseCamelCase
some.people.use.periods
And_aFew.People_RENOUNCEconvention

```

You can type the name of an object to view it. You can update the object at any time!



```{r}
this_is_a_really_long_name <- 2.5
this_is_a_really_long_name
```



#### Functions

R has lots of functions of this form `function_name(arg1 = val1, arg2 = val2, ...)`

Take a look at a basic function, `seq`. If you type it into R, note that it will help by adding parentheses, etc. When you make an assignment, you won't see the value. You'll have to ask R to print it.

```
seq(1,10)
x <- seq(1,10)
x

```

Or, you can speed things up: 

```

(x <- seq(1,10))

```



## Code-through

#### Reviewing data

Install and load the `nycflights1` package. Also load the `tidyverse`.

```
# install.packages("nycflights13")
library(nycflights)
library(tidyverse)
```

We're going to work with  `nycflights13::flights`. This **data frame** contains all 336,776 flights that departed from New York City in 2013. The data comes from the US [Bureau of Transportation Statistics](http://www.transtats.bts.gov/DatabaseInfo.asp?DB_ID=120&Link=0), and is documented in `?flights`.

```
flights
```

Why do we only see a bit of the data frame? It is very big. We are looking at a "[tibble](https://r4ds.had.co.nz/tibbles.html)," part of the `dplyr` universe, which shows the first 10 rows of a variable. It's a bit easier to work with. If you want to see all observations and variables, you can type `View()`.

One particular handy thing you can do is select one variable using `$`. 

```
flights$dep_delay
```

There are several types of data listed here: 

- `int` stands for integers.
- `dbl` stands for doubles, or real numbers.
- `chr` stands for character vectors, or strings.
- `dttm` stands for date-times (a date + a time).

#### Filter

`filter()` allows you to subset observations based on their values. The first  argument is the name of the data frame. The second and subsequent  arguments are the expressions that filter the data frame. For example,  we can select all flights on January 1st with:



```
filter(flights, month == 1, day == 1)
```

This will just display it but not change the data. You can create new data frames: 

```
jan1 <- filter(flights, month == 1, day == 1)
(dec25 <- filter(flights, month == 12, day == 25))
```



#### Logical operators

R using standard operators for comparisons: `>`, `>=`, `<`, `<=`, `!=` (not equal), and `==` (equal).

| Test        | Meaning                  |
| ----------- | ------------------------ |
| `x < y`     | Less than                |
| `x > y`     | Greater than             |
| `x == y`    | Equal to                 |
| `x <= y`    | Less than or equal to    |
| `x >= y`    | Greater than or equal to |
| `x != y`    | Not equal to             |
| `x %in% y`  | In (group membership)    |
| `is.na(x)`  | Is missing               |
| `!is.na(x)` | Is not missing           |

You can also use “or” with “`|`” and “not” with “`!`”:

| Operator | Meaning |
| -------- | ------- |
| `a & b`  | and     |
| `a | b`  | or      |
| `!a`     | not     |



Don't do this: 

```
filter(flights, month = 1)
filter(flights,month == 11 | 12)
```

Do this: 

```
filter(flights, month == 11) 

filter(flights, month == 11 | month == 12)

nov_dec <- filter(flights, month %in% c(11, 12))

```

#### Missing values

Often we will enounter missing values, or `NA`s (“not availables”). `NA` represents an unknown value so missing values are “contagious”: almost  any operation involving an unknown value will also be unknown.

```
NA > 5
#> [1] NA
10 == NA
#> [1] NA
NA + 10
#> [1] NA
NA / 2
#> [1] NA
```

If you want to determine if a value is missing, use `is.na()`:

```
is.na(x)
#> [1] TRUE
```



### Arrange rows with `arrange()`

`arrange()`changes the order in which rows are sorted. You can use multiple column names to break ties (ie sort by last name, then by first name). 

```
arrange(flights, year, month, day)

```

Use `desc()` to re-order by a column in descending order:

```
arrange(flights, desc(dep_delay))

```

Missing values are always sorted at the end:

```
df <- tibble(x = c(5, 2, NA))
arrange(df, x)
arrange(df, desc(x))

```

#### Selecting columns with `select()`

What if we have a bazillion variables. Then our friend `select()` will help us narrow things down.



```
# Select columns by name
select(flights, year, month, day)

# Select all columns between year and day (inclusive)
select(flights, year:day)

# Select all columns except those from year to day (inclusive)
select(flights, -(year:day))

```

There are a number of helper functions you can use within `select()`:

- `starts_with("abc")`: matches names that begin with “abc”.
- `ends_with("xyz")`: matches names that end with “xyz”.
- `contains("ijk")`: matches names that contain “ijk”.
- `matches("(.)\\1")`: selects variables that match a regular expression. This one matches any variables that contain repeated characters. I'm not going to talk about regular expressions, but if you know them from other languages, welcome!
- `num_range("x", 1:3)`: matches `x1`, `x2` and `x3`.

See `?select` for more details.

####  Rename 

Using  `rename()`  can help you rename variables

```
rename(flights, tail_num = tailnum)

```

Another option is to use `select()` in conjunction with the `everything()` helper. This is useful if you have a handful of variables you’d like to move to the start of the data frame.

```
flights_sml <- select(flights, 
  year:day, 
  ends_with("delay"), 
  distance, 
  air_time
)
mutate(flights_sml,
  gain = dep_delay - arr_delay,
  speed = distance / air_time * 60
)
```

---



We're going to work with [gapminder](https://www.gapminder.org/data/) [data](https://www.rdocumentation.org/packages/gapminder/versions/0.3.0)! This is just an excerpt of the data for simplicity, but we can play more later on.[^1]

You can bulk download some or all gapfinder data through various [repositories](https://www.gapminder.org/data/).

This block will install the gapminder package and load it. If this is your first time, you will need to "uncomment" the `install.packages` line in order to install it. You will want to comment it back out or delete it once it's installed, or it can create problems when knitting

```{r}
# install.packages("gapminder")
library(gapminder)
```

Now that we've loaded the library, we have access to a *data frame*

```{r}
gapminder
```

Let's look at the structure of our object

Note how there is a cool interactive window! Neat! 

---



[^1]: The full documentation is available [here](https://www.rdocumentation.org/packages/gapminder/versions/0.3.0)

 


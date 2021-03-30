# 09-01 Lesson: Fun with `ggplot2()`

## Lables

[Chapter 22: Titles, captions, and labels](https://clauswilke.com/dataviz/figure-titles-captions.html), *Fundamentals of data visualization*, Claus Wilke.



## Themes

Full walkthrough of each element of `ggplot2` themes from [Henry Wang](https://henrywang.nl/ggplot2-theme-elements-demonstration/)

Plus, this helpful infographic 



![theme_elements](/Users/emilybeam/Dropbox/EC137.S21/images/theme_elements.png)

### Standard themes: 

[Standard themes](https://ggplot2.tidyverse.org/reference/ggtheme.html): review of all 8 themes included w/ `ggplot2()`



### Packages

- [`ggthemes()`](https://github.com/jrnold/ggthemes) 
  - Additional documentation of possibilities with [`ggthemes()`](https://yutannihilation.github.io/allYourFigureAreBelongToUs/ggthemes/)
- [**hrbrthemes**](https://github.com/hrbrmstr/hrbrthemes)
- [**ggthemr**](https://github.com/cttobin/ggthemr)
- [**ggtech**](https://github.com/ricardo-bion/ggtech)
- [**tvthemes**](https://ryo-n7.github.io/2019-05-16-introducing-tvthemes-package/)
- [**ggpomological**](https://www.garrickadenbuie.com/project/ggpomological/) (trickier installation)

And of course, [there are more!](https://rfortherestofus.com/2019/08/themes-to-improve-your-ggplot-figures/)

Note: for some packages that include fonts, you will need to have the necessary fonts already on your system. For example `hrbrthemes` uses [Roboto Condensed](https://fonts.google.com/specimen/Roboto+Condensed?preview.text_type=custom) and a few others, and the beautiful `ggpomological` uses [Homemade Apple.](https://fonts.google.com/specimen/Homemade+Apple)





### Interactive theme editing

What?! 

Yes. 

Try it out with `ggThemeAssist()`

1. Install `ggThemeAssist`: `install.packages("ggThemeAssist")`
2. Load the library: `library(ggThemeAssist)`
3. Make a plot and save it as an object `myplot <- ggplot(data = stuff, mapping = ....)`
4. Call the plot: `myplot`
5. Highlight code that calls the plot with your mouse
6. Click on "add-ins" (see below)
7. Then select "ggplot Theme Assistant"
8. Go nuts!

<img src="/Users/emilybeam/Dropbox/EC137.S21/images/ggthemeassist.png" alt="ggthemeassist" style="zoom:50%;" />



### More resources on working with themes

[Figure Design](https://wilkelab.org/SDS375/slides/figure-design.html), Claus O. Wilke

## Colors

[Chapter 25: Using Colors in R](https://stat545.com/colors.html), Stat545: description of color palettes included in R and some background, plus examples. Plus, some intense detail on hexadecmial RGB and HCL

## Fonts

https://datavizm20.classes.andrewheiss.com/example/05-example/#bonus-ggthemeassist

## Other extensions

[All registered extensions](https://exts.ggplot2.tidyverse.org/gallery/) to `ggplot()`

[`DataExplorer`](https://www.rdocumentation.org/packages/DataExplorer/versions/0.8.2): Creates extremely detailed summary reports of key variables automatically! Jeez, Louise! 

## General principles

Few, Stephen. ["Grid lines in graphs are rarely useful."](http://www.perceptualedge.com/articles/dmreview/grid_lines.pdf) February 2005.





29 March 2021: 939 Wingspan

​							242 Ticket to ride


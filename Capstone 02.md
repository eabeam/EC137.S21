# Capstone 02 



**TLDR**; Make something similar to what you did for Capstone 01, but do it with R. Think about something related to inequality, but you can draw from Unit 01 topics if you prefer.

**Important:** You may work in groups of **two to three** on this Capstone. If you do, please notify me by e-mail in advance **before** the showcase so I can adjust small groups as needed.



## Research questions

### 1. Place-based inequality 

#### Question

1. Select a U.S. county of interest to you - this could be a place where you grew up, a place where you've spent substantial time, or a place that fascinates you (Youngstown, Ohio, anyone?)

2. Examine the patterns for a number of different groups (e.g., lowest income children, high income children) and outcomes (e.g., earnings in adulthood, incarceration rates).  You can do this exploration with the data you have, or in the [Opportunity Atlas](https://opportunityatlas.org/) itself. Then, select a few items to focus on

   **and/or**

​		Compare outcomes for those from your selected area to the entire United States 

3. You may also want to look for correlations between the outcomes you find and other factors, such as housing prices, income inequality, fraction of children with single parents, job density, etc.

4. When you present, take care to make sure you understand what data you are working with. What is the time period? How might neighborhoods have changed between then and now?  You may find it helpful to reference the full [Opportunity Atlas paper](https://opportunityinsights.org/wp-content/uploads/2018/10/atlas_paper.pdf).

#### Data

**Beginner/Intermediate**: Use this data set: [atlas.dta](atlas.dta). Note that you will need to install the `haven()` package to use the code `read_dta()` to import it. Restrict your entire analysis to the county you have chosen to focus on - so you will have one observation per census tract for that county.



You will find this [data description](atlas_datadescription.html) extremely helpful.

**Advanced**: You can download either County- or Census-tract data [here](https://opportunityinsights.org/data/). You would want to find the data corresponding to "The Opportunity Atlas: Mapping the Childhood Roots of Social Mobility" and then select the appropriate data depending on your level of analysis: 

​	Census Tract: "All Outcomes by Census Tract, Race, Gender and Parental Income Percentile "

​	County: "All Outcomes by County, Race, Gender and Parental Income Percentile"

​	You'll also see neighborhood/county characteristics that you can download and merge in.



In either case, you will find it useful to know your FIPS code. The easiest way to do this is within the mapper at [Opportunity Atlas](https://www.opportunityatlas.org/). For example, searching for “Lynwood Road, Verona, New Jersey” will display Tract 34013021000, Verona, NJ. The first two digits refer to the state code, the next three digits refer to the county code, and the last 6 digits refer to the tract code. 



####  Useful R Commands: 

Calculating unweighted summary statistics 

```r
# summary stats, unweighted  
summary(atlas$yvar) 
mean(atlas$yvar, na.rm=TRUE)
sd(atlas$yvar, na.rm=TRUE)
```

Calculating weighted summary statistics

*This is helpful is you want to compare your statistics to national data or to an average within your county or state . Why is it necessary to do it this way? If you average an outcome across all Census tracts, it will assign each tract an equal weight. That's an odd thing to do because some tracts have more people than others. When we use a weighted average, it essentially accounts for that.*

**Extremely brief example:** 

>  I have two tracts, one with a population of 5,000 where the poverty rate is 10%, and one where the population is 10,000 with a poverty rate of 20%. 
>
>  If I take an unweighted average: $\frac{10 + 20}{2} = 15$, implying a 15% average rate. But that's obviously not right! 
>
> If I take a weighted average: $\frac{5000*0.1 + 10000*0.2}{5000+10000} = 16.67$ , or a 16.7% rate. That seems better! 



```{r}
# Install and load package
install.packages("SDMTools")
library(SDMTools)

#Report weighted summary statistics*
wt.mean(atlas$yvar, atlas$count_pooled)
wt.sd(atlas$yvar,atlas$count_pooled)
```

Subset your variables

```{r}
## restrict observations to Wisconsin

wisconsin <- filter(atlas,state ==  55)

## restrict observations to Milwaukee  County

milwaukee <- filter(atlas,state ==  55 & county == 079
```

 



### 2. Global inequality: 

#### Question

How has inequality changed for countries in a particular region over time? 



3. Select a region of the world of interest to you. Examine how inequality has changed over time at the country level across various indicators. 
4. Explore the correlations between inequality and another potentially relevant factor, taking note that these explorations are not sufficient to give us evidence of causality. It could be GDP/capita, poverty rates, etc. 

#### Data

The World Bank [data repository](https://data.worldbank.org/) has excellent country-level data on inequality. You can download it directly and then import it into R, or you can use the  `WDI()` package. If you go for the package, you will want to spend some time with [the documentation](https://www.rdocumentation.org/packages/WDI/versions/2.7.3) to understand how to use it. 

### 3. Inequality in labor market outcomes in the U.S.

#### Questions

Explore trends in inequality in labor market outcomes (unemployment rates, labor force participation rates, wages) by demographic subgroups of your choosing.

#### Data

Recall that you can import just about any Excel sheet or .csv file into R! That means all the resources you used in Unit 01 (FRED, BLS, IPUMS, etc) are at your disposal.

To really step things up, check out Ray's demo of a neat package that lets you easily access BLS data! 

- R Markdown file: [BLSdemo-curtis.Rmd](BLSdemo-curtis.Rmd)
- Output: [BLSdemo-curtis.pdf](BLSdemo-curtis.pdf)
- Video demonstration (available on Blackboard embedded in Capstone 02 overview)

There is also some pretty easy-to-work with data embedded in a recent #TidyTuesday. See the description and links in the [08-01 PC for advanced users](https://eabeam.github.io/EC137.S21/R_preclass.html#advanced-user-n93)

*This is fairily similar to the Capstone 01 prompt! If you do this, make sure you are doing a substantially different topic from Capstone 01.*

### 4. Other

If you have another idea, run it by me first! I'm pretty open. 

To be suitable it must (a) have a clear connection to one of our topics in Units 1 or 2; (b) lend itself to analysis with data; (c) be substantially different from your Capstone 01 topic.



## Specifications

All the details are here! :point_down: :point_down: :point_down:

**Specifications powerpoint**	[pptx](Capstone2_Presentation.pptx)		[pdf](Capstone2_Presentation.pdf)

##### Deliverables

1. Slide deck as a PDF 
2. Slide deck as .pptx
3. Knit output file (pdf/html/docx) that contains: 
   - All code for all analysis
   - Capstone reflection with bibliography
   - Link to your video presentation

4. Data
   - Using a package: Skip this step, as you will call the data in your code!
   - Importing data: Include the raw .xlxs or .csv file
     - If it is fairly big - zip it first, is it better?
     - If it is massive – use [UVM FileTransfer ](https://filetransfer.uvm.edu/)and/or e-mail me


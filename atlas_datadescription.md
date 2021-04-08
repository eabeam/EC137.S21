# DATA DESCRIPTION, FILE: `atlas.dta`

 

The data consist of *n* = 73,278 U.S. Census tracts. For more details on the construction of the variables included in this data set, please see [Chetty, Raj, John Friedman, Nathaniel Hendren, Maggie R. Jones, and Sonya R. Porter. 2018. “The Opportunity Atlas: Mapping the Childhood Roots of Social Mobility.” NBER Working Paper No. 25147](https://opportunityinsights.org/wp-content/uploads/2018/10/atlas_paper.pdf). 

 

## **Table 1**

**Definitions of Variables in `atlas.dta`**

 

| **Variable name**                                            | **Label**                                                    | **Obs.** |
| ------------------------------------------------------------ | ------------------------------------------------------------ | -------- |
| (1)                                                          | (2)                                                          | (3)      |
| ***1. Geographic identifiers\***                             |                                                              |          |
| *tract*                                                      | Tract FIPS Code (6-digit) 2010                               | 73,278   |
| *county*                                                     | County FIPS Code (3-digit)                                   | 73,278   |
| *state*                                                      | State FIPS Code (2-digit)                                    | 73,278   |
| *cz*                                                         | Commuting Zone Identifier (1990 Definition)                  | 72,473   |
|                                                              |                                                              |          |
| ***2. Characteristics of Census  tracts\***                  |                                                              |          |
| *hhinc_mean2000*                                             | Mean Household Income 2000                                   | 72,302   |
| *mean_commutetime2000*                                       | Average Commute Time of Working Adults in 2000               | 72,313   |
| *frac_coll_plus2010*                                         | Fraction of Residents with a College Degree or  More in 2010 | 72,993   |
| *frac_coll_plus2000*                                         | Fraction of Residents with a College Degree or  More in 2000 | 72,343   |
| *foreign_share2010*                                          | Share of Population Born Outside the U.S.                    | 72,279   |
| *med_hhinc2016*                                              | Median Household Income in 2016                              | 72,763   |
| *med_hhinc1990*                                              | Median Household Income in 1999                              | 72,313   |
| *popdensity2000*                                             | Population Density (per square mile) in 2000                 | 72,469   |
| *poor_share2010*                                             | Poverty Rate 2010                                            | 72,933   |
| *poor_share2000*                                             | Poverty Rate 2000                                            | 72,315   |
| *poor_share1990*                                             | Poverty Rate 1990                                            | 72,323   |
| *share_black2010*                                            | Share black 2010                                             | 73,111   |
| *share_hisp2010*                                             | Share Hispanic 2010                                          | 73,111   |
| *share_asian2010*                                            | Share Asian 2010                                             | 71,945   |
| *share_black2000*                                            | Share black 2000                                             | 72,368   |
| *share_white2000*                                            | Share white 2000                                             | 72,368   |
| *share_hisp2000*                                             | Share Hispanic 2000                                          | 72,368   |
| *share_asian2000*                                            | Share Asian 2000                                             | 71,050   |
| *gsmn_math_g3_2013*                                          | Average School District Level Standardized Test  Scores in 3rd Grade in 2013 | 72,090   |
| *rent_twobed2015*                                            | Average Rent for Two-Bedroom Apartment in 2015               | 56,607   |
| *singleparent_share2010*                                     | Share of Single-Headed Households with Children  2010        | 72,564   |
| *singleparent_share1990*                                     | Share of Single-Headed Households with Children  1990        | 72,196   |
| *singleparent_share2000*                                     | Share of Single-Headed Households with Children  2000        | 72,285   |
| *traveltime15_2010*                                          | Share of Working Adults w/ Commute Time of 15  Minutes Or Less in 2010 | 72,939   |
| *emp2000*                                                    | Employment Rate 2000                                         | 72,344   |
| *mail_return_rate2010*                                       | Census Form Rate Return Rate 2010                            | 72,547   |
| *ln_wage_growth_hs_grad*                                     | Log wage growth for HS Grad., 2005-2014                      | 51,635   |
| *jobs_total_5mi_2015*                                        | Number of Primary Jobs within 5 Miles in 2015                | 72,311   |
| *jobs_highpay_5mi_2015*                                      | Number of High-Paying (>USD40,000 annually)  Jobs within 5 Miles in 2015 | 72,311   |
| *nonwhite_share2010*                                         | Share of People who are not white 2010                       | 73,111   |
| *popdensity2010*                                             | Population Density (per square mile) in 2010                 | 73,194   |
| *ann_avg_job_growth_2004_2013*                               | Average Annual Job Growth Rate 2004-2013                     | 70,664   |
| *job_density_2013*                                           | Job Density (in square miles) in 2013                        | 72,463   |
|                                                              |                                                              |          |
| ***3. Measures of Upward Mobility  from the Opportunity Atlas\*** |                                                              |          |
| *kfr_pooled_p25*                                             | Household income ($) at age 31-37 for children  with parents at the 25th percentile of the national income distribution | 72,011   |
| *kfr_pooled_p75*                                             | Household income ($) at age 31-37 for children  with parents at the 75th percentile of the national income distribution | 72,012   |
| *kfr_pooled_p100*                                            | Household income ($) at age 31-37 for children  with parents at the 100th percentile of the national income distribution | 71,968   |
| *kfr_natam_p25*                                              | Household income ($) at age 31-37 for Native  American children with parents at the 25th percentile  of the national income distribution | 1,733    |
| *kfr_natam_p75*                                              | Household income ($) at age 31-37 for Native  American children with parents at the 75th percentile of the national income  distribution | 1,728    |
| *kfr_natam_p100*                                             | Household income ($) at age 31-37  for Native American children with parents at  the 100th percentile of the national income distribution | 1,594    |
| *kfr_asian_p25*                                              | Household income ($) at age 31-37  for Asian children with parents at the 25th  percentile  of the national income  distribution | 15,434   |
| *kfr_asian_p75*                                              | Household income ($) at age 31-37  for Asian children with parents at the 75th  percentile of the national income distribution | 15,360   |
| *kfr_asian_p100*                                             | Household income ($) at age 31-37  for Asian children with parents at the 100th  percentile of the national income distribution | 13,480   |
| *kfr_black_p25*                                              | Household income ($) at age 31-37  for Black children with parents at the 25th  percentile  of the national income  distribution | 34,086   |
| *kfr_black_p75*                                              | Household income ($) at age 31-37  for Black children with parents at the 75th  percentile of the national income distribution | 34,049   |
| *kfr_black_p100*                                             | Household income ($) at age 31-37  for Black children with parents at the 100th  percentile of the national income distribution | 32,536   |
| *kfr_hisp_p25*                                               | Household income ($) at age 31-37  for Hispanic children with parents at the 25th  percentile  of the national income  distribution | 37,611   |
| *kfr_hisp_p75*                                               | Household income ($) at age 31-37  for Hispanic children with parents at the 75th  percentile of the national income distribution | 37,579   |
| *kfr_hisp_p100*                                              | Household income ($) at age 31-37  for Hispanic children with parents at the 100th  percentile of the national income distribution | 35,987   |
| *kfr_white_p25*                                              | Household income ($) at age 31-37  for White children with parents at the 25th  percentile  of the national income  distribution | 67,978   |
| *kfr_white_p75*                                              | Household income ($) at age 31-37  for White children with parents at the 75th  percentile of the national income distribution | 67,968   |
| *kfr_white_p100*                                             | Household income ($) at age 31-37  for White children with parents at the 100th  percentile of the national income distribution | 67,627   |
|                                                              |                                                              |          |
| ***3. Counts of number of  children under 18 in 2000 (to calculate weighted summary statistics)\*** |                                                              |          |
| *count_pooled*                                               | Count of all children                                        | 72,451   |
| *count_white*                                                | Count of White children                                      | 72,451   |
| *count_black*                                                | Count of Black children                                      | 72,451   |
| *count_asian*                                                | Count of Asian children                                      | 72,451   |
| *count_hisp*                                                 | Count of Hispanic children                                   | 72,451   |
| *count_natam*                                                | Count of Native American children                            | 72,451   |

 

*Note:* This table describes the variables included in the atlas.dta file.
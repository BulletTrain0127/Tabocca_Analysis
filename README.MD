# Tobacco Analysis

### What is Exploration Idea?

The objective of this analysis is to understand how tobacco use or smoking affects monthly premium rates. Furthermore, it is interesting to explore how premium rates vary for smokers and non-smokers in different states over years from 2014 to 2016.


### Why Does it Matter?

Under the health care law, insurance companies can charge tobacco users up to 50 percent more in premiums. According to healthcare.gov, while some states are charging the maximum 50 percent for smokers, seven states including California, New York and New Jersey prohibit  
tobacco use surcharges completely. The Tobacco surcharge has become a very controversial topic in the healthcare insurance industry. Some people think the surcharge encourage smokers to quit while others argue that surcharge creates financial burden and makes the coverage  
unaffordable to individuals. I think it would be interesting to explore how different states react to the tobacco surcharge and what the variations in surcharge are at the state level in the  United States.

## Methodology 

 **1. Get Data**
 This analysis uses “Rate.csv” (https://www.kaggle.com/hhs/health-insurancemarketplace#Rate.csv)

 **2. Data Cleaning**
During the step of data cleaning, the primary tasks include checking data type, checking missing values and outliers, imputing values if necessary.

**3. Exploratory Data Analysis**
In order to understand the distribution of data, it is useful to calculate some descriptive statistics such as mean, median, standard deviation, minimum and maximum.

**4. Comparing Individual Rate and Individual Tobacco Rate over Years**
To see the changes in rates from 2014 to 2016, it is helpful to compare the median individual rates and the median individual tobacco rates. A side-by-side histogram can be used to visualize the rates for both smokers and non-smokers.

**5.  Comparing Individual Rate and Tobacco Rate across States**
First of all, it is helpful to sort the states based on the median individual rates in descending order for each year between 2014 and 2016. The same steps can be performed on the median individual tobacco rates as well. Then a side-by-side bar plot that combines all three years rates can be used to demonstrate the changes over time.


 
## Outstanding Concerns with the Analysis Plan

1. Since this dataset only covers the time period from 2014 to 2016, some changes or trends in the premium rates may not be quite significant.

2. Depending on the nature of the data distribution, the comparison between states based on the median individual rates may present some bias, even though it is better than the comparison using the mean individual rates as the mean is significantly influenced by outliers.

3. In the dataset, I’m not sure whether the tobacco preference is the only difference between the Individual Rate and Individual Tobacco Rate. Since the original source of the dataset does not explicitly explain, there might exist some other factors which are not strictly controlled and may lead to the differences in the premium rates.

4. Some states may have more observations for different plans when some states may only have few records. For example, some states may have data for all three years between 2014 and 2016 while some states may only have records for the year of 2015. In such way, the state-level comparison may present some bias.


## Findings & Conclusions

The dataset covers a total of **16,808 health insurance plans from 39 states** in the United States. However, not all of 39 states have records for all three years between 2014 and 2016. The dataset does not include records for the following states: *New York, Colorado, Vermont,
Maryland, California, Massachusetts, Rhode Island, Kentucky, Washington, Minnesota, Connecticut and Washington, D.C.*

**Virginia** has very spread out distributions for the individual rate between 2014 and 2016. According to the research (https://www.theatlantic.com/health/archive/2018/04/the-city-withthe-most-expensive-aca-insurance-in-the-united-states/558605/), Charlottesville, Virginia is the city with the most expensive ACA Insurance in the United States. The primary reason for such high premiums is that there is only one individual-market carrier in Charlottesville.

![enter image description here](https://github.com/BulletTrain0127/Tobacco_Analysis/blob/master/plot1.PNG?raw=true)

The above bar plot demonstrates the median individual rate and the median individual tobacco rate from 2014 to 2016. The median rate for non-smokers shows an **increasing trend** from 2014 to 2016. In contrast, the median rate for smokers remains **relatively stable** compared to rates for non-smokers.

![enter image description here](https://github.com/BulletTrain0127/Tobacco_Analysis/blob/master/plot2.PNG?raw=true)

The above plot shows the changes on the median individual rate by state from 2014 to 2016. Among 39 states in the dataset, most states experience **a significant **increase**** on the median individual rate between 2014 and 2016.

![enter image description here](https://github.com/BulletTrain0127/Tobacco_Analysis/blob/master/plot3.PNG?raw=true)

The above bar plot demonstrates the changes on the median individual tobacco rate by state from 2014 to 2016. **Alaska** experiences **a dramatic increase** on the median individual tobacco rate between 2014 and 2016 while **Indiana** has a completely opposite pattern.

![enter image description here](https://github.com/BulletTrain0127/Tobacco_Analysis/blob/master/plot4.PNG?raw=true)

**Alaska** has the highest median individual rate between 2014 and 2016. On the other side, **Kansas, Michigan** and **New Mexico** rank the bottom 3 in terms of the median individual rate.

![enter image description here](https://github.com/BulletTrain0127/Tobacco_Analysis/blob/master/plot5.PNG?raw=true)

In addition, **Wyoming** and **Alaska** has the highest median individual tobacco rates between 2014 and 2016. On the other side, **Kansas, Utah** and **Oregon** rank the bottom 3 in terms of themedian individual tobacco rate.

According to the research, Alaska is one of the states which allow insurance companies to charge the maximum 50 percent tobacco surcharge on smokers under the ACA. In fact, Alaska medical costs are more than double the national average (https://www.premera.com/PremeraVoices/All-Posts/Alaska-medical-costs-are-more-than-double-the-national-average/). The possible reasons for such high costs in Alaska include small population and isolation from larger markets, limited number of providers and higher compensation for providers.

## Next Steps for Further Analysis
1. If I have data about the premium rates for multi-individual plans with allowed dependents who are smokers, then it is possible to determine whether the tobacco surcharge is different for individual plans and for multi-individual plans.

2. Only 39 of 50 states in the United States are included in the dataset. If we have complete data for all the states, the state-level analysis could be more comprehensive.

3. If I have data about smoking rate for each state, then we can check whether the state smoking rate is correlated to the premium rates for smokers and to see the changes in the relationship over years.

4. For this analysis, I did not exclude dental-only plans since the rates for dental plans would also be affected by tobacco use. However, it is worthwhile to look at dental-only plans separately and to analyze the tobacco surcharge on dental-only plans. Then we are able to better understand how the impact of tobacco surcharge vary on the rates of dental-only plans and the rate of full health coverage plans.

5. Electronic cigarettes like JUUL, serving as smoking alternative, become very popular to younger generation. According to the news, the U.S. Food and Drug Administration plans to regulate Electronic cigarettes and vapor products in the future. I am curious how insurance
companies evaluate the use e-cigarette users and how the use of e-cigarette may impact the insurance rates. If there exists such impact, how does it look like compared to the tobacco surcharge? 
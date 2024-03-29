# Home Values Difference versus School Rating in New Jersey 

# Project Description/Outline: 
    #Data analysis of real estate information and school district ratings to identify trends in the market
    #Observe charted data to determine possible correlations between school ratings and home prices

# Research Questions to Answer:
#### How much higher are average home prices in districts with better ranked schools?
#### How has the current school ranking affected neighboring home values over the last 20 years?
#### What is the relationship between school district metrics and the amount of low income families in the population?


    
# Data Used and Analyzed
#### Zillow Housing Data (CSV)

#### Great Schools Neighborhood Data (Web Scraping)

        
# Conclusions
### Longitudinal
![Home Prices](Outputs/Change_in_home_price.png)
####  This graph charted the average home value for three different categories of school rating (<6, 6-8, 8+) for the last 20 years. The ANOVA test revealed an f-value of 15.532 which exceed the critical value -- this suggests that these groups are different in a significant manner. When looking at the graph, it is evident that the better the school district, the higher the average school price is over the last 20 years. 
![Avg Home Values](Outputs/Change_in_home_price_vs_avg.png)
####  These values represent the dollar value that a great, good, or below average school district creates against the average home value in New Jersey. For example, the below average school districts have houses that are ~$70k cheaper than the average 2020 home. Using the ANOVA method, we determined the f-value (91.6) to exceed the critical value; thus these groups have some statistically significant difference.

#### Notably, these differentials are not steady even though the previous graph shows that all three categories demonstrated the same general shape. The below average school district is becoming cheaper ($37k vs $70k less). The good school district fluctuated up and down in the last 20 years but has stayed around $100k more in the last 15. The value of a great school district in 2000 was $165k but now these same districts cost in excess of $300k more than average. 

### Recent Data
![Bar for School Ratings](Outputs/bar_rating_vs_value.png)
####  Looking at the most recent Zillow data, a house in a poor school district averages around $365k, a good district costs about $570k, and the top tier of school districts run over $800k. 
![2019](Outputs/school_rating_vs_2019_value.png)
![2020](Outputs/school_rating_vs_2020_home_value.png)
![2021](Outputs/school_rating_vs_2021_home_value.png)
####  When completing a scatter plot for each year and a linear regression, we see a weak correlation between home value and school rating. Each year had a R-Value around 0.33. This r-value illustrates that there is likely other factors in play when considering home value. These variables may include related items such as crime rate, access to groceries, walkability, etc. In future analysis, we could correct for square footage and room count by zooming in on a few specific school districts.

### Low Income Households
![Low income bar](Outputs/low_income.png)
####  Although home price is a good proxy for general wealth, we can also use the percentage of low income students in a school to investigate more directly whether the average income of a district affects its rating and thus its home values. 

#### In an exploration of the school districts in our dataset, the bar graph illustrates heavily right-tailed distribution. In other words, there are many more school districts with less low income students.

![Low income bar](Outputs/school_rating_vs_Low_income.png)
#### In our regression of percentage of low income students and school rating, there is a moderate negative correlation (r-value = 0.48). Once we cross over to districts with a percentage over 60%, none of the areas have a school rating of Good or Great (6-8, 8+). In other words, none of the highly performing school districts in New Jersey contain a majority of low income students. 
![Rating vs Value](Outputs/Home_Value_and_Ranking_by_county.png)
####  As we zoom out to the county level, the trends for home value and school rating hold steady. As the school ratings get better, so too do the average home values. 

## Final Conclusions:
##### According to recent Zillow data, homes in poor school districts average around $365,000, while those in good districts cost about $570,000, and properties in top-tier districts exceed $800,000. Analysis using scatter plots and linear regression revealed a weak correlation between home value and school rating, with an R-value of around 0.33 consistently across years. This indicates that factors beyond school quality, such as crime rates, access to amenities, and neighborhood walkability, likely impact home values.

##### Over the past two decades, the price gap between below-average and good school districts has widened, with below-average districts now priced approximately $70,000 lower than the average house. Good districts have consistently commanded a premium of around $100,000 over below-average ones for the past fifteen years. Furthermore, the value of great school districts has soared, with prices now exceeding $300,000 more than the average house, underscoring the enduring importance of quality education in the housing market.

##### In our analysis correlating the percentage of low-income students with school ratings, we found a moderate negative correlation (r-value = 0.48). Specifically, when examining districts with a percentage of low-income students exceeding 60%, none of them achieved a school rating of Good or Great (6-8, 8+). Put simply, high-performing school districts in New Jersey typically do not have a majority of low-income students.


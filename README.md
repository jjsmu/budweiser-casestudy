*Presentation for the CEO and CFO of Budweiser (group1-6)*


- add links for: 
- Recorded Presentation
- Slides
- Code

Introduction:

Subject: Comprehensive Data Analysis Report and Strategic Insights

Dear CEO and CFO,

I am delighted to present to you our comprehensive data analysis report, meticulously compiled to offer valuable insights that will guide our strategic decision-making processes. Our team has diligently worked to distill complex statistical findings into clear, actionable information, ensuring that the content is accessible and immediately applicable, regardless of one’s statistical background.

The data entrusted to us has been meticulously examined, employing a range of statistical techniques tailored to uncover the underlying patterns, trends, and anomalies. Our analysis aims to illuminate aspects of our operations and market engagements that are performing exceptionally well, while also pinpointing areas that may warrant a closer look or a strategic pivot.

In crafting this report, we have remained cognizant of the imperative to communicate our findings in a manner that transcends the complexities of statistical jargon. We have striven to ensure that each insight is articulated clearly, supported by visual aids where necessary, and contextualized within our broader business landscape.

We believe that the findings enclosed herein will not only validate our current strategic directions but also unveil opportunities for innovation, efficiency, and growth. We are confident that this report will serve as a valuable tool in our collective endeavor to fortify Budweiser’s market leadership and foster sustained prosperity.

I am eager to delve into the details of our findings and discuss how we can translate these insights into concrete actions that align with our strategic objectives. Your insights and directives have been invaluable in this process, and I am keen to ensure that this analysis serves as a robust foundation for our ongoing collaborative efforts.

Thank you for entrusting us with this important task. I look forward to our continued partnership and the mutual success that lies ahead.

Best regards,

Group 6

Purpose:

## Summary Memo: Analysis of Breweries and Beer Data
*Objective:* The analysis aims to provide insights into the breweries' distribution, beer characteristics, and the relationship between beer bitterness and alcohol content.

*Breweries Distribution:* We will determine the number of breweries present in each US state.

*Data Merging:* The beer data will be merged with the breweries' data. 

*Handling Missing Data:* We will address the missing values across all columns for the purpose of this analysis, we treaded the missing data as MCAR (Missing Completely At Random). Please note, many of the missing values pertained to IBU. 

*Beer Characteristics by State:* We'll compute and visualize the median alcohol content (ABV) and bitterness (IBU) for beers in each state using a bar chart.

*State with Extreme Beer Traits:* Identification of states producing the most alcoholic and bitter beers will be determined.

*ABV Analysis:* An analysis and commentary on the distribution and summary statistics of the ABV variable will be provided.

*Bitterness vs. Alcohol Content:* A scatter plot will be drawn to examine the relationship between beer bitterness (IBU) and its alcohol content (ABV). An interpretative analysis will follow.

*KNN Classification for IPAs vs. Other Ales:* Using the KNN classification method, we'll investigate the differences in IBU and ABV between IPAs (India Pale Ales) and other types of Ale. While KNN is our primary method, we remain open to integrating other analytical approaches for a more comprehensive understanding.

*Additional Insights:* In a bid to provide Budweiser with a unique value proposition, we will derive an additional inference from the data, substantiating its importance with statistical evidence.
This analysis is designed to provide Budweiser with a thorough understanding of the U.S. craft beer landscape, guiding future strategic decisions

**Summary memo written using Chat-GPT** 

# Codebook For Budweiser Case study

Data sets obtained from Client:
[Beers](https://github.com/BivinSadler/MSDS_6306_Doing-Data-Science/blob/Master/Unit%208%20and%209%20Case%20Study%201/Beers.csv) 
& 
[Breweries](https://github.com/BivinSadler/MSDS_6306_Doing-Data-Science/blob/Master/Unit%208%20and%209%20Case%20Study%201/Breweries.csv)



Also saved in this repository as of October 9, 2023:
[Beers](https://github.com/jjsmu/group16/blob/main/Beers.csv) & 
[Breweries](https://github.com/jjsmu/group16/blob/main/Breweries.csv)



**Notes:** 
- -The datasets provided consist of information on 2410 US craft beers and 558 US breweries with details such as beer name, ABV, IBU, and brewery location. 

-The Key variable that connects the data sets is Brewery_id in Beer.csv and Brew_ID in Brewery.csv. We renamed variables to have matching column names in order to merge.

-We assumed data was missing at random, and filtered out missing values when doing analysis. This is detailed in the EDA.rmd file. 

-Refer to EDA.rmd file for code relating to merging, transformation and analysis. 

**Data Dictionary for Beer:**

| Variable   | Label                                       | Data Type | Missing Data Code | Example Values                                          |
|---------------|---------------|---------------|---------------|---------------|
| Name       | Name of Beer                                | String    | empty cells       | Blood Orange Gose, Summer Solstice Cerveza Crema (2009) |
| Beer_ID    | unique identifier for beer                  | Integer   | empty cells       | 35,767,1712                                             |
| ABV        | Indicated alcohol by volume (percentage)    | Decimal   | empty cells       | 0.09,0.125                                              |
| IBU        | International Bitterness Units (percentage) | Integer   | empty cells       | 92,17,4                                                 |
| Brewery_id | unique identifier for brewery               | Integer   | empty cells       | 409,2,73                                                |
| Style      | Style of beer                               | Nominal   | empty cells       | 409,2,73                                                |
| Ounces     | amount of beer in indivisual can/bottle     | Integer   | empty cells       | 12,8.4,16                                               |

**Data Dictionary for Brewery:**

| Variable | Label                                              | Data Type | Missing Data Code | Example Values                           |
|---------------|---------------|---------------|---------------|---------------|
| Brew_ID  | unique identifier for brewery                      | Integer   | empty cells       | 1,20,558                                 |
| Name     | Name of Brewery                                    | String    | empty cells       | NorthGate Brewing, Avery Brewing Company |
| City     | City where brewery is located                      | String    | empty cells       | Seven Points, Portland                   |
| State    | U.S. state (abbreviation) where brewery is located | String    | empty cells       | MN,MI, CO                                |


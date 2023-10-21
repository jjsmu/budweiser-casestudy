*Presentation for the CEO and CFO of Budweiser (group1-6)*
- [Presentation Slides](https://github.com/jjsmu/group16/blob/main/Group_6_Budweiser_Casestudy_01.pdf)
- [Presentation Recording](https://smu.zoom.us/rec/share/r9-9Y3vzjyNYPyWkb0vkyWsP19tHeI7tMli1XtIW6XjIHpj6nZBq2PemOKPACtgl.QlkdbGwch0Q6zC9N)
  
### Purpose: Budweiser Casestudy 01 
- This case study examines the distributions and center of mean and median values for all beers sold by breweries listed in the dataset. The two datasets: Beers.csv and Breweries.csv contains  are combined to study the relationship between alcohol by content and bitterness to understand the current trends in the alcohol beverage industry.  

## Summary Memo: Analysis of Breweries and Beer Data
*Objective:* The analysis aims to provide insights into the breweries' distribution, beer characteristics, and the relationship between beer bitterness and alcohol content.

*Breweries Distribution:* We will determine the [number of breweries present in each US state.](https://github.com/jjsmu/group16/blob/main/state_counts.csv)

*Beer Characteristics by State:* We'll compute and visualize the median alcohol content (ABV) and bitterness (IBU) for beers in each state using a bar chart.

*State with Extreme Beer Traits:* Identification of states producing the most alcoholic and bitter beers will be determined.

*ABV Analysis:* An analysis and commentary on the distribution and summary statistics of the ABV variable will be provided.

*Bitterness vs. Alcohol Content:* A scatter plot will be drawn to examine the relationship between beer bitterness (IBU) and its alcohol content (ABV). An interpretative analysis will follow.

*KNN Classification for IPAs vs. Other Ales:* Using the KNN classification method, we'll investigate the differences in IBU and ABV between IPAs (India Pale Ales) and other types of Ale. 

*Additional Insights:* In a bid to provide Budweiser with a unique value proposition, we will derive an additional inference from the data (in regards to naming conventions and size of beers,) to provide Budweiser with a thorough understanding of the U.S. craft beer landscape, guiding future strategic decisions

**Summary memo written with aid of Chat-GPT** 

### Code
- [RMD file](https://github.com/jjsmu/group16/blob/main/EDA.rmd)
- [HTML file](https://github.com/jjsmu/group16/blob/main/EDA.html)
# Codebook For Budweiser Case study


# OS
- R version 4.3.1 (2023-06-16 ucrt)
- Platform: x86_64-w64-mingw32/x64 (64-bit)
- Running under: Windows 10 x64 (build 19045)

# Data
- *Data sets* 
- Data sets obtained from Client:
[Beers](https://github.com/BivinSadler/MSDS_6306_Doing-Data-Science/blob/Master/Unit%208%20and%209%20Case%20Study%201/Beers.csv) 
& 
[Breweries](https://github.com/BivinSadler/MSDS_6306_Doing-Data-Science/blob/Master/Unit%208%20and%209%20Case%20Study%201/Breweries.csv)

-  Also saved in this repository as of October 9, 2023:
[Beers](https://github.com/jjsmu/group16/blob/main/Beers.csv) & 
[Breweries](https://github.com/jjsmu/group16/blob/main/Breweries.csv)

-  The datasets provided consist of information on 2410 US craft beers and 558 US breweries with details such as beer name, ABV, IBU, and brewery location. 


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

## Data preparation

-  *Data Merging:* The beer data will be merged with the breweries' data. 

-  *Handling Missing Data:* We will address the missing values across all columns for the purpose of this analysis, we treaded the missing data as MCAR (Missing Completely At Random). Please note, many of the missing values pertained to IBU. Filtering is addressed in the EDA. rmd file

- *Key variable:* The Key variable that connects the data sets is Brewery_id in Beer.csv and Brew_ID in Brewery.csv. We renamed variables to have matching column names in order to merge.

- Refer to [EDA.rmd](https://github.com/jjsmu/group16/blob/main/EDA.rmd) file for code relating to merging, transformation and analysis. 
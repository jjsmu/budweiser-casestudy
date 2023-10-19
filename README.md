*Presentation for the CEO and CFO of Budweiser (group1-6)*


- add links for: 
- Recorded Presentation
- Slides
- Code & Explanation 




*DELETE BEFORE SUBMISSION: Codebook: The code book is an explanation of concepts or definitions needed to know to understand the data and reproduce the analysis. This could include the machine and operating system the project was run on, a data dictionary of the data, any transformations or feature creation performed with the data, merging details, or any other pieces of general information that someone should know about the environment and data. For this project thecodebook should be a Word doc or pdf or could be the ReadMe file in your GitHub repo.(

# Codebook For Budweiser Case study

Data sets obtained from Client:
[Beers](https://github.com/BivinSadler/MSDS_6306_Doing-Data-Science/blob/Master/Unit%208%20and%209%20Case%20Study%201/Beers.csv)
&
[Breweries](https://github.com/BivinSadler/MSDS_6306_Doing-Data-Science/blob/Master/Unit%208%20and%209%20Case%20Study%201/Breweries.csv)

Also saved in this repository as of October 9, 2023:
[Beers](https://github.com/jjsmu/group16/blob/main/Beers.csv)&
[Breweries](https://github.com/jjsmu/group16/blob/main/Breweries.csv)


**Notes:** 

-The Key variable that connects the data sets is Brewery_id in
Beer.csv and Brew_ID in Brewery.csv. We renamed variables to
have matching column names in order to merge.

-We assumed data was missing at random, and removed those observations with missing values.

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


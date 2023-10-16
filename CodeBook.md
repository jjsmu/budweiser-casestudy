# Codebook For Budweiser Case study

Data sets obtained from Client:
[Beers](https://github.com/BivinSadler/MSDS_6306_Doing-Data-Science/blob/Master/Unit%208%20and%209%20Case%20Study%201/Beers.csv)
&
[Breweries](https://github.com/BivinSadler/MSDS_6306_Doing-Data-Science/blob/Master/Unit%208%20and%209%20Case%20Study%201/Breweries.csv)

Also saved in this repository as of October 9, 2023:
[Beers](https://github.com/jjsmu/group16/blob/main/Beers.csv)&
[Breweries](https://github.com/jjsmu/group16/blob/main/Breweries.csv)

*Note: the Key variable that connects the data sets is Brewery\_id in
Beer.csv and Brew\_ID in Brewery.csv. Will need to rename variables to
have matching column names in order to merge.*

Data Dictionary for Beer:

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th>Variable</th>
<th>Label</th>
<th>Data Type</th>
<th>Missing Data Code</th>
<th>Example Values</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Name</td>
<td>Name of Beer</td>
<td>String</td>
<td>empty cells</td>
<td>Blood Orange Gose, Summer Solstice Cerveza Crema (2009)</td>
</tr>
<tr class="even">
<td>Beer_ID</td>
<td>unique identifier for beer</td>
<td>Integer</td>
<td>empty cells</td>
<td>35,767,1712</td>
</tr>
<tr class="odd">
<td>ABV</td>
<td>Indicated alcohol by volume (percentage)</td>
<td>Decimal</td>
<td>empty cells</td>
<td>0.09,0.125</td>
</tr>
<tr class="even">
<td>IBU</td>
<td>International Bitterness Units (percentage)</td>
<td>Integer</td>
<td>empty cells</td>
<td>92,17,4</td>
</tr>
<tr class="odd">
<td>Brewery_id</td>
<td>unique identifier for brewery</td>
<td>Integer</td>
<td>empty cells</td>
<td>409,2,73</td>
</tr>
<tr class="even">
<td>Style</td>
<td>Style of beer</td>
<td>Nominal</td>
<td>empty cells</td>
<td>409,2,73</td>
</tr>
<tr class="odd">
<td>Ounces</td>
<td>amount of beer in indivisual can/bottle</td>
<td>Integer</td>
<td>empty cells</td>
<td>12,8.4,16</td>
</tr>
</tbody>
</table>

Data Dictionary for Brewery:

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th>Variable</th>
<th>Label</th>
<th>Data Type</th>
<th>Missing Data Code</th>
<th>Example Values</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Brew_ID</td>
<td>unique identifier for brewery</td>
<td>Integer</td>
<td>empty cells</td>
<td>1,20,558</td>
</tr>
<tr class="even">
<td>Name</td>
<td>Name of Brewery</td>
<td>String</td>
<td>empty cells</td>
<td>NorthGate Brewing, Avery Brewing Company</td>
</tr>
<tr class="odd">
<td>City</td>
<td>City where brewery is located</td>
<td>String</td>
<td>empty cells</td>
<td>Seven Points, Portland</td>
</tr>
<tr class="even">
<td>State</td>
<td>U.S. state (abbreviation) where brewery is located</td>
<td>String</td>
<td>empty cells</td>
<td>MN,MI, CO</td>
</tr>
</tbody>
</table>

------------------------------------------------------------------------

Directions delete eveythig under this line at end. Codebook: The code
book is an explanation of concepts or definitions needed to know to
understand the data and reproduce the analysis. This could include the
machine and operating system the project was run on, a data dictionary
of the data, any transformations or feature creation performed with the
data, merging details, or any other pieces of general information that
someone should know about the environment and data. For this project the
codebook should be a Word doc or pdf or could be the ReadMe file in your
GitHub repo.

What is a codebook? A codebook provides information on the structure,
contents, and layout of a data file. Users are strongly encouraged to
review the codebook of a study before downloading the data file(s).

Although codebooks vary widely in quality and amount of information
given, a typical codebook includes:

Column locations and widths for each variable Definitions of different
record types Response codes for each variable Codes used to indicate
nonresponse and missing data Exact questions and skip patterns used in a
survey Other indications of the content and characteristics of each
variable Additionally, codebooks may also contain:

Frequencies of response Survey objectives Concept definitions A
description of the survey design and methodology A copy of the survey
questionnaire Information on data collection, data processing, and data
quality The body of a codebook describes the content of the data file.
The following elements are generally included for each variable in the
data file:

Variable Name: Indicates the variable number or name assigned to each
variable in the data collection. Variable Column Location: Indicates the
starting location and width of a variable. If the variable is a
multiple-response type, then the width referenced is that of a single
response. Variable Label: Indicates an abbreviated variable description
(maximum of 40 characters) that can be used to identify the variable. In
some cases, an expanded version of the Variable Name can be found in a
Variable Description List. Missing Data Code: Indicates the values and
labels of missing data. If “9” is a missing value, then the codebook
could note “9 = Missing Data.” Other examples of missing data labels
include “Refused,” “Don’t Know,” “Blank (No Answer),” and “Legitimate
Skip.” Some analysis software requires that certain types of data be
excluded from analysis and designated as “Missing Data,” (i.e.,
inappropriate, not ascertained, not ascertainable, or ambiguous data
categories). Users can use these “Missing Data” codes as needed. Code
Value: Indicates the code values occurring in the data for a variable.
Value Label: Indicates the textual definitions of the codes.
Abbreviations commonly used in the code definitions are “DK” (“Don’t
Know”), “NA” (“Not Ascertained”), and “INAP” (“Inapplicable”).

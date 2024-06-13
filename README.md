## Residential Housing Analysis for Bay Area
## Objective
1.Analyze the current real estate listings data for Bay area counties 

2.Understand the current housing market dynamics to answer questions as

-Most listed real estate class in Bay area* (*Santa Clara County, San Mateo County, Alameda County, Contra Costa County, Marin County, Napa County, San Francisco County, Solano County and Sonoma County)


-Can most households affords those listings based on current financial situation

-Cities where real estate listings are showing downward financial trend

## Approach

1.Source

-zip code data from government website (https://www.unitedstateszipcodes.org/zip-code-database/)

-Property listings data from realtor.com (approx 900 listings with 500+ in cities of interest)

-Household data from government census data website* 

2.Load

-Zipcode - manual one time download 

-Property Listings - scrape the realtor.com for the properties listed for zip codes in the counties of Bay area

-Income Data - Government census data website.

3.Process

-Remove the listings where the information is corrupt based on the json parsing.

-Consider the median household income only for analysis. 

-Analyze on top 20 cities based on the number of listings we could get

## Distribution Of Property Types In Top 20 Cities of Bay Area

Work:
Used matplotlib.pyplot for better visualization
Grouping the data by city and property type and plot barh chart

Analysis💡:
In San Francisco, almost 50% of the property type is condo & 30% is single family home

In San Jose, around 40% are single family & 20% are condo properties

Almost every other city has approximately higher percentage of single-family homes as property type

## Most Popular Home Type In Bay Area

Work:
Value count on home type column and plot pie chart

Analysis💡:
Single family is the most popular home type in the Bay Area with 53.6%
Around 80% of the properties listed on the market are single family and condos together

Which reinforces for the fact that the current market needs are categorizing to more nuclear families in the top 20 cities based on the listing count of the data.

## SQFT vs Price & Distribution of SQFT in Listings

Analysis💡:

The scatter plot shows the overall listing price vs sqft distribution. Sqft and list price shows linear correlation

Almost 90% of the properties are less than 3000 sqft.

Most of the listed properties are 1500-2000 sqft; shows single family or condo listing concentration

## Affordability of Housing in Bay Area Cities

1 Bed : Most Bay area cities affordable due to high median income 

2 Beds :  Still affordable with SF, Berkeley, Napa being exceptions

3 Beds: Still accessible for those further from the bay area

4 Beds: Exclusive to HNI’s, ultra rich with Brentwood still an exception

## Summary

Good Deals
-Available in major hustling cities like San Francisco, San Jose, Oakland, & Santa Rosa 

High-Priced Properties- Cities like Fremont, Hayward, Fairfield, Walnut Creek 

Unsustainable to Own- Almost all the Bay Area
prominent cities with a few exceptions of Brentwood, Concord, Vacaville, Antioch, and Vallejo

Price Affordability- Market catering to the needs by listing single family homes & condos with ~80% of the total listings 

Recommendation- Cities such as Fremont with its close proximity to major hubs and high median household income






































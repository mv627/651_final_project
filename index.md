
# Nasha Virata GIS 651 Final Project 

This project is inspired by Wachsmuth and Weisler’s paper ["Airbnb and the Rent Gap"](https://upgo.lab.mcgill.ca/publication/airbnb-and-the-rent-gap/airbnb-and-the-rent-gap.pdf) examining Airbnb and the rent gap  and Duvisac, Baiocchi, and Vantu’s paper ["Behind Gentrification’s Gloss"](https://journals.sagepub.com/doi/abs/10.1177/15365042221107656). 

I was intrigued by Wachsmuth and Weisler's findings that Airbnb listings can be taken as drivers of a new form of rent gap, and therefore one metric to indicate gentrification in New York City. For this project however, I am making a simpler level of analysis by comparing the average prices of airbnb listings per neighborhood to two other ways to measure neighborhood differences: gross median rent and 311 calls concerned with housing. 

First, I took data from the [US Census](https://data.census.gov/) on gross median rent as a percentage of household dollars in NYC in 2019. The hashed values indicate the areas that register as parks.

![Gross Median Rent](http://github.com/mv627/651_final_proj.github.io/blob/main/gross_med_rent.png?raw=true)

The second map clips the Housing Related 311 calls during the period of September 1-7, 2022 to the New York neighborhoods map. The dataset itself was filtered for processing and memory-related purposes. THe reason I map out 311 calls though was because I wanted to find out if there was a similar finding with airbnb listings and 311 calls as is found in the Duvisac et al paper. There, the authors want to understand not so much displacement (which Wachsmuth et al is more concerned with) but what happens to those left behind. They do this by looking at the type of housing-related 311 calls and find that substandard housing conditions are in gentrifiying areas and not just low-income. This is borne out my the map below. However, the reasons for these calls may be due to more than just housing conditions and may reflect selection bias and the type of resident willing to make calls in the first place. It would be good to study this further and over a longer time period.  
![Housing Related 311 Calls, September 1-7, 2022](http://github.com/mv627/651_final_proj.github.io/blob/main/311_calls.png?raw=true)

For the third interactive map, I used a spatial join to create an interactive map of the average prices per neighborhood. If we compare to the other two maps, we that there are clear correlations in places that bear a higher burden of rent (Upper Manhattan, the Bronx, and Central Brooklyn), the 311 related housing calls and the average prices of Airbnbs in the neighborhood. 

http://github.com/mv627/651_final_proj.github.io/blob/main/avg_price_neighborhood.html

For the next steps, I'd like to do more on understanding 311 calls, with a larger dataset and look at all of these datasets over a defined period in time rather than a simple snapshot. Formatting wise, I would display these as layers. 

Credit due to: https://medium.com/analytics-vidhya/folium-and-choropleth-weird-names-cool-graph-4f9b99b99190
Data sources:
http://insideairbnb.com/
https://data.census.gov/
https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9

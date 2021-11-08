# Zillow Observed Rent Index (ZORI)

This index is a smoothed measure of the typical observed market rate rent across a given region. ZORI is a repeat-rent index that is weighted to the rental housing 
stock to ensure representativeness across the entire market, not just those homes currently listed for-rent. The index is dollar-denominated by computing 
the mean of listed rents that fall into the 40th to 60th percentile range for all homes and apartments in a given region, which is once again weighted 
to reflect the rental housing stock.

The reason behing choosing the zillow data set is to better visualize the rental data for past few years across different months in order to better figure out the 
rental price and the way it varies during a year. One can base their decisions of when to actually rent and the tenure of the lease to sign in order to save on rent.
The reason that I choose this viz is since I did struggle for 2-3 months to find a home within my budget and decide on the tenure of the rental lease I signed. Having
access to the data and visualization would turn out to be useful while going through the appartment hunt!

### Data Visualization and Source 

Below is a vizualization from ZORI (zillow observed rental index) data set which represents the increase in total rent in major metro cities within the United States.
The viz is trying to represent the trend in some of the major cities from the year 2005 to 2019. One thing that the vizualization prominently represents is the increase
in rent through each year.

Some key Insights: All-in-all, U.S. renters paid roughly $4.5 trillion in rent during the 2010s, capped off with $512 billion in 2019 alone.

The total amount of money spent on rent nationwide over the past 10 years is higher than the GDP of Germany (a shade less than $4 trillion in 2018), the world’s fourth-largest 
national economy. Total rent paid in 2019 alone is higher than the entire 2018 GDP of Thailand ($505 billion) and just short of Argentina’s ($518 billion).

<div class="flourish-embed flourish-bar-chart-race" data-src="visualisation/1078503"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Please refer the link for access to full data: [Data](https://files.zillowstatic.com/research/public_csvs/zori/Metro_ZORI_AllHomesPlusMultifamily_SSA.csv?t=1636241110)

### WireFraming the solution

As discussed in the critique, since we have such data available at our disposal, we can use it to generate better and more valuable insights. One problem that I would try to 
address using this data would be for the audience/people who are looking to rent an apartment in one of the metro cities in the United States. The data viz can help these
people to select the month in which they would like to rent to get the best rent for themselves and also to decide on a lease if they have to move urgently. For example,
somebody who has to move urgently can take shorter lease in exepnsive months and then look for apartments with less rent in months when the rent trend indicates the rent to
be low. This same can also be used by landlords who generally rent their apartments in deciding the changes within the rent prices.

In order to acheive the final solution, below are some of the intermediate wireframes created to move towards the final goal.

### Total rent trend (2014-2019)

First wireframe I was thinking to visualize using vertical bar chart has been created which essentially points out the trend of total rent across 106 cities every month. The data is averaged out over all years but instead decided to use a line chart has been drawn for multiple countries and end user has the flexibility to scan through data for different years. This wireframe is representing represent every city on one single chart with different color schemes as the rent donmination increases.

![image](https://user-images.githubusercontent.com/37357639/140671714-bc33e8b4-bcbe-4659-b7b7-692cc4f963bd.png)

In the below final wireframe, I have decided on the solution to provide end user the flexibility to finally choose between cities and represented the cumulative data on
different cities in the US. The reason for choosing a line chart is to represent the time series on the monthly front. The rent has been averaged out across the years.

![image](https://user-images.githubusercontent.com/37357639/140671756-370b520c-2516-4e9a-a2af-b6311df73ed7.png)


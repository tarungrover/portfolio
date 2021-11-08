# Zillow Observed Rent Index (ZORI)

This index is a smoothed measure of the typical observed market rate rent across a given region. ZORI is a repeat-rent index that is weighted to the rental housing 
stock to ensure representativeness across the entire market, not just those homes currently listed for-rent. The index is dollar-denominated by computing 
the mean of listed rents that fall into the 40th to 60th percentile range for all homes and apartments in a given region, which is once again weighted 
to reflect the rental housing stock.

The reason behind choosing the zillow data set is to better visualize the rental data for past few years across different months in order to better figure out the 
rental price and the way it varies during a year. One can base their decisions of when to actually rent and the tenure of the lease to sign in order to save on rent.
The reason that I choose this viz is since I did struggle for 2-3 months to find a home within my budget and decide on the tenure of the rental lease I signed. Having
access to the data and visualization would turn out to be useful while going through the appartment hunt!

### Data Visualization and Source 

Below is a vizualization from ZORI (zillow observed rental index) data set which represents the increase in total rent in major metro cities within the United States.
The viz is trying to represent the trend in some of the major cities from the year 2005 to 2019. One thing that the vizualization prominently represents is the increase
in rent through each year.

#### PLEASE NOTE:The viz was created by taking the product of the estimated number of renter households and the summed ZRIs for each metro

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

##### Total rent trend (2014-2019)

First wireframe I was thinking to visualize using vertical bar chart has been created which essentially points out the trend of total rent across 106 cities every month. The data is averaged out over all years but instead decided to use a line chart has been drawn for multiple countries and end user has the flexibility to scan through data for different years. This wireframe is representing represent every city on one single chart with different color schemes as the rent donmination increases.

![image](https://user-images.githubusercontent.com/37357639/140671714-bc33e8b4-bcbe-4659-b7b7-692cc4f963bd.png)

In the below final wireframe, I have decided on the solution to provide end user the flexibility to finally choose between cities and represented the cumulative data on
different cities in the US. The reason for choosing a line chart is to represent the time series on the monthly front. The rent has been averaged out across the years.

![image](https://user-images.githubusercontent.com/37357639/140684969-7d1e3a7f-2cc2-4a28-94e5-aba02f8b4e33.png)

### Testing the Solution

I did share the initial wireframe with a couple of people and realized that representing many countries on one graph would cause problem in readibility and creating a grid 
would also not enable any comparisons. Hence, I mention the details about feedback of the final wireframe since the initial wireframe was rejected.

On sharing the final wireframe created above, the below feedback was received as per the questions asked. I have taken and considered feedbacks from 2 people, person X and Y.

#### Person X

- *Can you tell me what you think this is?*
The first thing that the person X recognized was option to select different cities and the next thing the graph talks about the rents in different months. 

- *Can you describe to me what this is telling you?*
Person X mentioned that the graph shows that lowest possible rent can be attained around months March-June and recognized that as the best time to move in.

- *Is there anything you find surprising or confusing*
One thing that year being mentioned as (2014-2019) is this rent the summation of all or averaged across the years?

- *Who do you think is the intended audience for this*
People who are new to the country and looking to rent an appartment.

- *Is there anything you would change or do differently?*
Person X mentioned that this can also be depicted using a histogram (or a form of bar) as well and would  have liked to see it instead.

- *Would you like to see the dots or just a normal line?*
Person X mentioned that points help them map it to a particular month and they would like to see them and also maybe in a different color to different intensities of the dot 
size that represent the lowering of rent.

- *Could this have been better if bar graphs are used instead?*
yes, bars would look better and also maintain this to be a time series trend effectively.

#### Person Y

- *Can you tell me what you think this is?*
The first thing that Person Y noticed was the fesaibility to select different cities and this viz talks about the rent trends across years 2014-2020.

- *Can you describe to me what this is telling you?*
This talks about different rent trends across 6 years and divides it on the basis of months.

- *Is there anything you find surprising or confusing?*
One thing that Person Y brought to my attention was that their initial intrepretation after reading the title was that they saw the amount of rent paid that people paid during each month which is also correct in a way.

- *Who do you think is the intended audience for this?*
As mentioned by the person, the intended audience would be people looking to rent the apartments and could help them figure out the month in which the rents would be the 
lowest and could also help the people figure out their rental contract tenures.

- *Is there anything you would change or do differently?*
The person said that they would definitely mention the fact that rents are lowered at some places of the graph which could be advantageous for people who are looking for new 
places.

- *Would you like to see the dots or just a normal line?*
The dots are good enough since that helps them map to the month.

- *Could this have been better if bar graphs are used instead?*
Yes, a bar graph does show the intensity of the quantity since ti would show me how much effect and lower excatly each month is as compared to the other one.

***LEARNINGS/CHANGES***

After noticing the similarities and opinions from different peopel, I would be changing the following things to make my message through the data visualization much more 
clearer:
1. A clearer title that does not only specify total rent but also the catches the eye of intended audience.
2. Mention if the digits are actually average or summation over the sepcified year.
3. Consider the vertical bar graph for each month and see how it actually looks.
4. Specifically highlights the month with least average rent to attract immediate attention of people paying rent which would be the intended audience.
5. Data points for each month are necessary if I am not using bars to represent the rise and fall.

### Final Solution'

The below is the final data visualization that I have created. I have used a line chart and scaled y-axis according to scale. This cahrt could finally help people scan through multiple metro cities in US and visually compare when the rents are actually lowest during an year. The rents are averaged across the years (2014-2020). It also represents the average rent of entire United States as well and also gives an opportunity to select for one particular city. Feel free to explore different cities and enjoy.

On conlcusion that we can make from the data viz below is that a person can alsmost save 50-60$ on a monthly basis if they rent an apartment in United States during January and sign a contract of an year or more.

<div class="flourish-embed flourish-chart" data-src="visualisation/7768876"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Thank You!


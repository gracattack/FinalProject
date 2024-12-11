---
layout: default
---

### Introduction 

	
&emsp;For our analysis project, we analyzed the relationship between regular-season playing time distributions and final rankings of WNBA teams. Our goal is to determine if there is a specific method of determining playing time that is the most successful. Do successful teams only play their best players the majority of the game, or do they utilize their entire bench and evenly distribute the load? We aim to determine if any successful playing time patterns exist and visualize them if they do. 

&emsp;The data used in this project is taken from the WNBA Statistics page, the official website for all of the league’s statistics. Our goal was to look at data from the past 5 seasons (2020-2024) which required building a dataset of our own. We had access to data sorted by individual season of every player's average per-game statistics. To begin, we downloaded each of the 5 sets of regular season data and added it to a separate sheet in an Excel workbook. Then we read each season in Colab and created individual dataframes. To each data frame, we added a column for the respective year. This was helpful later when we merged the data sets. The next step was to add the rankings that each player’s respective team finished at the end of the season. Using data from ESPN, we added the final team rankings to each dataset for each player. We then proceeded to merge the data frames to have one large dataset from 2020 to 2024. Finally, we got rid of some excess statistics columns that we did not need for our analysis to keep our data as small and as workable as possible. The process was repeated for playoff data. 

&emsp;The first part of our analysis project was constructing the dataset to be usable in the way we wanted. The second part was to look at the distribution of average playing time for each team across 5 years and see if we could detect any successful patterns both during the regular season and playoffs. We created a graph for each WNBA team with 5 distributions representing the 5 years observed. Each graph has average playing time on the x-axis and density on the y-axis. The density represents how many times a playing time was observed among players in the team. We included the final rank the team ended the season with and commented on any patterns we observed. Additionally, the playoff distributions for the teams who eventually won the championship are commented on. We also created plots of the 5 teams who finished first, last, and became champions each year and looked for patterns in their average playing time per game distributions. 








### LinkedIn

[Gracie Maulik Linkedin](https://www.linkedin.com/in/gracie-maulik-195049262)

# Project Portfolio

### Where's Schueller?

Below is an embedded plot of where Schueller was on May 31st, 2024.

{% include_relative may_31.html %}

### Data Sources and Project Ideas

#### 1.) Basketball Data

> Data: [Basketball Reference](https://www.basketball-reference.com/wnba/teams/)

> This website has data from the NBA and WNBA on all players and teams including individual game statistics and team statistics. It would be fascinating to look at different player's average statistics (points per game, rebounds per game, etc.) and compare that to how the team has performed. It would also just be cool to convert the data into a time series and plot a player's performance over time. One other idea that Carly had was to visualize the areas on the court where players have made the most shots and determine their optimal shooting location.

#### 2.) UN Environmental Data

> Data: [UN Environmental Data (under the Environment Tab)](https://data.un.org)

> The environmental datasets look at $CO_2$ emissions, threatened species, and water supply/sanitation coverage per country. Using this data, it would be cool to explore each country's numbers and compare them to economic indicators over time, such as GDP per capita. This potentially would show the overall health of the country and it would be interesting to see if the environmental and economic parts of the country are related. 

#### 3.) Census Data

> Data: [United States Census Database](https://data.census.gov/)

> This database has all of the census data from the United States, including demographic information and population counts. I think it would be interesting to compare different indicators with each other, such as population over time and poverty over time. The data could be resampled to have the same time series and could be plotted on the same graph to see if there were any visible relationships. 

#### 4.) Economic Indicators Data

> Data: [World Bank Economic Indicators](https://databank.worldbank.org/)

> The database above has loads of data on all countries across the world on everything from GDP per capita to mortality rates. It is an overwhelmingly large dataset, but one that could be used to compare to other datasets addressed above. US GDP per capita over the years can be tied in with census data or human poverty levels per country can be compared to the $CO_2$ emissions that a country produces. 

#### 5.) Presidential Data and the Bureau of Labor Statistics

> Data: [Bureau of Labor Statistics](https://data.bls.gov/dataQuery/search)

> This dataset contains US data on the unemployment rate and job growth. It would be fascinating to take the years of each presidential administration and compare each presidencies unemployment rate and job growth. It is always an issue that Republicans cite as their main factor for voting, it would be interesting to see if Republican presidents have done more for the economy than Democrats or vice versa.

### Above and Beyond

To further practice embedding plots onto my page, I have included Scheuller's location data for May 30th, 2024. 

{% include_relative may_30.html %}


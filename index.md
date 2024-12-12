---
layout: default
---

### Introduction 

	
&emsp;For our analysis project, we analyzed the relationship between regular-season playing time distributions and final rankings of WNBA teams. Our goal is to determine if there is a specific method of determining playing time that is the most successful. Do successful teams only play their best players the majority of the game, or do they utilize their entire bench and evenly distribute the load? We aim to determine if any successful playing time patterns exist and visualize them if they do. 

&emsp;The data used in this project is taken from the WNBA Statistics page, the official website for all of the league’s statistics. Our goal was to look at data from the past 5 seasons (2020-2024) which required building a dataset of our own. We had access to data sorted by individual season of every player's average per-game statistics. To begin, we downloaded each of the 5 sets of regular season data and added it to a separate sheet in an Excel workbook. Then we read each season in Colab and created individual dataframes. To each data frame, we added a column for the respective year. This was helpful later when we merged the data sets. The next step was to add the rankings that each player’s respective team finished at the end of the season. Using data from ESPN, we added the final team rankings to each dataset for each player. We then proceeded to merge the data frames to have one large dataset from 2020 to 2024. Finally, we got rid of some excess statistics columns that we did not need for our analysis to keep our data as small and as workable as possible. The process was repeated for playoff data. 

&emsp;The first part of our analysis project was constructing the dataset to be usable in the way we wanted. The second part was to look at the distribution of average playing time for each team across 5 years and see if we could detect any successful patterns both during the regular season and playoffs. We created a graph for each WNBA team with 5 distributions representing the 5 years observed. Each graph has average playing time on the x-axis and density on the y-axis. The density represents how many times a playing time was observed among players in the team. We included the final rank the team ended the season with and commented on any patterns we observed. Additionally, the playoff distributions for the teams who eventually won the championship are commented on. We also created plots of the 5 teams who finished first, last, and became champions each year and looked for patterns in their average playing time per game distributions. 

### Methods and Results: Individual Teams

_Atlanta Dream:_

![Atlanta Dream](https://github.com/user-attachments/assets/b5a8e5f6-6521-419f-badb-dcf5569f4c0d)

&emsp;The Atlanta Dream changed its strategy drastically from 2020 to 2021, going from a flatter distribution and utilizing stronger players more to uniform time for everyone. This did not help their ranking in those seasons, as they went from 10th to 11th. 2022 also saw fairly even playing time amongst all players and a return to 10th place. In 2023 and 2024, the distribution shifts to peak below 20 minutes and become wider, indicating that the majority of players saw less than half of the game, but some outliers had higher playing amounts. Their ranking increased in these years as well, to 5th and 8th.

_Chicago Sky:_ 

![Chicago Sky](https://github.com/user-attachments/assets/cc6c2f04-bf44-4b0c-a5c8-ba8b0e8ef72e)

&emsp;The Chicago Sky have seen their fair share of success throughout the last five years. Their playing time distributions for the regular season between their best season (2022) and their worst season (2024) are quite different. The distribution of playing time in 2022 was bimodal with peaks in minutes around 28 and 10 minutes. This indicates a mix of traditional “star” players who are on the floor for more minutes at a time and “role/bench”  players who act more as support players. In this year, the Sky appeared to rely more on their star players as that peak is higher than that of the role players. This could indicate a lack of trust in the bench or the high-caliber play from the team's best players. In 2024, their worst season as of late, the Sky played more players giving out fewer minutes in the process. This could indicate a rebuilding year for the team. The Sky could be trying to foster more players at once and get them more experience. In fact, the Sky received two first-round draft picks in Angel Reese and Kamilla Cardoso in 2024 and the distribution of playing time alludes to the potential strategy to foster chemistry and experience in this young team. The average number of minutes played per game that year was 18.19.

![Chicago Sky Playoffs](https://github.com/user-attachments/assets/5f18d1ba-ddf9-4990-8ffd-a6f7c0a91ce2)

&emsp;However, Chicago’s best playoff run was in 2021, the team entered the playoffs as the 6th seed and came out with a championship. Their distribution in playing time from the regular season into the playoffs saw a dramatic shift. The team went from a narrow single-peaked distribution to a more uniform, bimodal distribution. The number of minutes played 25th percentile in the regular season was 11.9 compared to the 25th percentile in the playoffs 7.4. Similarly, the 75th percentile of playing time in the regular season was 26.2 compared to 32.55 in the playoffs.  The Sky changed their strategy entering the playoffs and relied proportionally on their star and bench players. Their stars consistently played around 25-30 minutes compared to the bench’s 5-10 minutes. The bimodal shape of the distribution also reflects the consistency of playing time among the players. 



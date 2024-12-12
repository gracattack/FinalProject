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

_Connecticut Sun:_ 

![Connecticut Sun](https://github.com/user-attachments/assets/186b9c7f-1547-4c1a-b6cf-03ec315b03db)

&emsp;The Connecticut Sun finished with their worst ranking in the past 5 years in 2020 at 7th. The distribution was bell-shaped and peaked around 15 minutes. The next 4 years show multiple peaks, with the highest around 30 minutes and the lower peak less than 10 minutes. This shows that there is unequal playing time on this team with some people playing close to full games and others barely leaving the bench. This strategy appears to work for the Sun as they entered the playoffs in first place in 2021 and have placed 3rd in the years since.

_Dallas Wings:_

![Dallas Wings](https://github.com/user-attachments/assets/a839369f-cdba-4201-8aa3-872dd67541f2)

&emsp;The distribution of playing time in 2020 was incredibly steep and peaked around 20 minutes, indicating that most players saw half of the game. The team finished 9th this year, showing it might not be a great strategy. The distributions continually get flatter as years go on, indicating that some players are seeing higher average playing times and others are seeing lower averages. From 2021 to 2023, the Wings increased their ranking each year, only to fall to 11th in 2024.

_Indiana Fever:_

![Indiana Fever](https://github.com/user-attachments/assets/3affc504-8d1f-4e33-846c-7227e64ff332)

&emsp;The 2024 WNBA season saw the Indiana Fever have their best performance in recent years. The team ended the regular season in 6th place and made the playoffs for the first time in eight years. Their best season had their athletes playing an average of 19.44 minutes and showed a narrow unimodal distribution. This showcases the organization’s strategy of having their players play a similar amount of time. They only have a few players who average more than 19.44 minutes and only a few who average less. The distribution shows less distinguishable groupings than other teams.

&emsp;However, this does not appear to be a new tactic for the Fever. 2024 had a similar distribution of playing time compared to previous seasons indicating a growth in chemistry and ability to work together as a team. There were no drastic changes in terms of playing time thus indicating that there must have been a change in the caliber of players the fever brought in and/or the cohesion of the team on the court. 

_Las Vegas Aces:_

![Las Vegas Aces](https://github.com/user-attachments/assets/4a4c1c89-e93e-4578-9c4d-0db420cbf153)

&emsp;The Aces have been one of the premier teams in the WNBA over the last few years finishing the regular season in first place three of the last five years. Their worst performance in recent years was in 2024 when they finished the regular season in fourth place. During this time, they had fewer players who played large minutes and more who played fewer minutes. Their 2024 distribution was also one of their widest. It has the largest standard deviation of the Aces' last five seasons at 12.023667 minutes. This could indicate a lack of consistency in minutes played or the coaches want to extend minutes to her bench players and provide them with valuable experience. A wide range of playing times could also indicate injuries and the coaches attempt to fill the gaps of those players.  

![Las Vegas Aces Playoffs](https://github.com/user-attachments/assets/1d40ebe7-2ab7-48cf-a8bb-3d3376c15125)

&emsp;That said, the Aces have won two championships in the last three years. Both years, in the playoffs, they had bimodal distributions. This again alludes to the strategy of playing the star players the majority of the game while sprinkling in role players to provide invaluable support. The bimodal distribution again implies that the coaches are consistent with the number of minutes they hand out to each player. In 2020 and 2021, where they finished the regular season first and second respectively. However, the Aces did not come away with a championship either year (in 2021 they didn’t even make the title game) and their playoff playing time distributions are drastically different than when they did. Both years have extremely narrow distributions, with standard deviations of 10.278946 and 10.195882 respectively, and are unimodal distributions. This indicates that the Aces either relied too heavily on their star players and did not have the bench support necessary to win a championship or played their star players and bench players a similar amount, not effectively utilizing the weapons at their disposal.  

&emsp;Las Vegas also didn’t win the championship in 2024 but did employ the same bimodal distribution of playing time as their previous, championship seasons. However, the Aces did enter the playoffs as the fourth seed. This could indicate the possible lack of cohesion in the regular season carrying over to the playoffs. Additionally, between 2023 and 2024, the team lost two-time league MVP and starter Candace Parker to retirement/injury leaving the team to fill the massive void she left. So while the bimodal playing time distribution proved very effective in 2022 and 2023, it didn’t translate to championship success in 2024. 

_Los Angeles Sparks:_

![Las Angeles Sparks](https://github.com/user-attachments/assets/40b0a52d-71c4-48cb-b149-34c88fb545da)

&emsp;Above is the Los Angeles Sparks playing time distribution over the past 5 seasons. Also included is the final ranking the team finished at the end of each year. The Sparks had incredibly similar distributions in 2021 and 2023, but they finished near the bottom in both years. The team had a more uniform distribution in 2022 and 2024 but finished second-to-last and last in those years respectively. The only year they finished well was in 2020 where they finished 3rd. The distribution is uniform and peaks at lower average minutes than the rest of the distributions, indicating that the playing time was uniform on the team and that they relied more on their bench and subbed consistently.

_Minnesota Lynx:_

![Minnesota Lynx](https://github.com/user-attachments/assets/07144403-5d31-4390-b2bb-191dc0e14b6f)

&emsp;The Minnesota Lynx are a historically good WNBA franchise and have made the playoffs four of the last five years. They also appear to have some of the most consistent distributions of playing time among WNBA teams in the last five years. All distributions are narrow and have one distinct peak. Excluding 2022, the average number of minutes per game played ranged from 18.16 to 19.46 and the standard deviation ranged from 8.74 to 10.79 minutes per game. The 2022 season has the highest peak of all Lynx distributions at around 15 minutes per game. The Lynx therefore had more players playing fewer minutes than stars playing large minutes. This is to be expected because in 2022, the Lynx’s best player,  Napheesa Collier, who finished second in the MVP race in 2024, missed the majority of the season due to maternity leave. Therefore the Lynx had to adjust to her absence, playing more role players around 10-20 minutes a game. This rotation of players only playing 15 minutes a game may not allow them to “get their footing” and feel comfortable within lineups. The combination of this and the absence of their best player led to the worst Lynx finish in the last five years: ending the season in ninth place and missing the playoffs altogether. 

_New York Liberty:_

![New York Liberty](https://github.com/user-attachments/assets/e441a106-0bdc-42df-a89f-12c322a0371b)

&emsp;New York in 2020, 2021, and 2022 were consistently finished towards the bottom of the rankings, 12th (last), 8th, and 7th respectively. Each of the corresponding regular-season distributions is quite narrow and with peaks closer to 20-30 minutes a game. In 2020 especially, the highest peak was around 25 minutes a game. The average number of minutes played per game in 2020, 2021, and 2022 were 20.26, 21.65 and 20.25 respectively. Additionally, their respective standard deviations were 6.44, 7.76 and 7.72. This is a strong indication that the Liberty relied heavily on a few players to take most of the minutes. 
 
&emsp;However, they saw success in 2023 and 2024, finishing the season in 2nd and 1st respectively. These distributions are drastically different from the three previous ones. They are much wider with standard deviations of 11.101061 and 10.619108 respectively. Both the 2023 and 2024 were much more uniform, indicating that the team had some star players mixed in with a healthy amount of role players. Additionally, they relied on them equally and consistently. 

![New York Liberty Playoffs](https://github.com/user-attachments/assets/f2a9418f-72b5-4d49-a7ca-1f1b1dac94a7)

&emsp;In both 2023 and 2024, the New York Liberty made it to the championship game, winning it in 2024. While their regular season distributions were quite uniform, their successful playoff distributions were again bimodal. During their title run, the Liberty consistently played their star players more minutes while sprinkling in their role players. They relied equally on both groups with their stars consistently playing 25-45 (higher than 40 because two of the games went into overtime) and bench players playing 5-15 minutes per game. 

_Phoenix Mercury:_

![Phoenix Mercury](https://github.com/user-attachments/assets/713f3c64-8456-4c6f-8052-2e504ede5baa)

&emsp;In 2020, the Phoenix Mercury had a high distribution of players averaging around 20 minutes per game where they finished 5th. In 2021, they also finished 5th, but with a much flatter distribution and utilizing longer playing time for some players. 2022, 2023, and 2024 all have two peaks, one around 10 minutes and one around 30 minutes, indicating that players either played most of the game or a small part. Few played about half of the game. Their ranking decreased as this pattern started, finishing in 8th, 12th, and 7th place in the past three years.

_Seattle Storm:_

![Seattle Storm](https://github.com/user-attachments/assets/30587ddf-e53a-47bd-9f28-a95779a2ffb7)

&emsp;The Seattle Storm do not follow consistent patterns in their playing time distributions. In 2020, they finished 2nd and had a very narrow distribution around 20 minutes. In 2021, they had a much wider distribution, indicating more variation in playing time. In 2022, they had significant peaks around 30 minutes and a narrower distribution once again. In 2023, they follow more of the pattern from 2021, which saw them their worst ranking by far in the last 5 years. Finally, in 2024, the distribution is much flatter and spread out, indicating players had different playing time averages all across the team.

![Seattle Storm Playoffs](https://github.com/user-attachments/assets/7d261c55-c5d2-4546-a15b-d97fcaaf3a8b)

&emsp;The storm won the championship in 2020 when they entered the playoffs as the two seed. During their successful 2020 run, they had a large number of players playing around 5-15 minutes per game with fewer playing between 20 and 35 minutes. Additionally, in 2020, their regular season distribution did not change much in shape when the team entered the playoffs. This is most likely due to how the 2020 season was structured. The COVID-19 pandemic was running rampant during this time and therefore, the 2020 WNBA season was condensed and isolated. Instead of the normal 40 regular season games, the 2020 “Bubble” season was only 20 games. Because there were fewer games played in the regular seasons, teams did not need to manage the workload of their star players as much as they would in a season that is double in length. This meant that their lineups could be more consistent in playing time because there was less concern for long-term fatigue. Therefore, the distributions of the regular season and playoffs look more similar to each other than other seasons. 




















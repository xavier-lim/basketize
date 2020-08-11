# Basketize
![Basketize Header](https://github.com/xavier-lim/basketize/blob/master/images/basketize_header.jpg)

Basketize is an optimization model whose main objective is to minimize an NBA team's salary while achieving key team statistics likely to lead to wins. It uses an exploratory data analysis (EDA) and mixed-integer optimization (MIO) to determine which combination of 12 players will collectively lead the NBA in all team statistics likely to lead to wins. The model is also used to determine which free agent players the Toronto Raptors should target in the 2020 offseason to maximize their chance of winning.

Although their team payroll for the 2019-2020 season is about $3 million less than the average NBA team, the Raptors will be in a tough predicament this offseason since Pascal Siakam signed a contract that would increase his salary by about $27 million for the 2020-2021 season. In addition, the Raptors have multiple key players who will become free agents (Gasol, Ibaka, VanVleet). Ultimately, it is unlikely the Raptors will be able to re-sign all their players in the offseason, unless a player takes a major pay cut. Hence, I decided to apply my Basketize model to the Raptors.

To view the article I wrote about my model on LinkedIn, please visit: [Basketize: Optimizing Basketball Rosters](https://www.linkedin.com/pulse/basketize-optimizing-basketball-rosters-xavier-lim/)

## Table of Contents
1.	[Project Tools](https://github.com/xavier-lim/basketize#project-tools)
2.	[Data Sources](https://github.com/xavier-lim/basketize#data-sources)
3.	[Power BI Project Dashboards](https://github.com/xavier-lim/basketize#power-bi-project-dashboards)
4.	[Conclusion](https://github.com/xavier-lim/basketize#conclusion)
5.	[Acknowledgements](https://github.com/xavier-lim/basketize#acknowledgements)
6.	[Author](https://github.com/xavier-lim/basketize#author)

## Project Tools
*     Julia - [Download Julia](https://julialang.org/downloads/) 
*     Jupyter Notebook - To create a Jupyter Notebook, open Julia and insert the following lines of code

      ```
      julia> using IJulia()
      julia> notebook()
      ```
      
*	NBA Player Statistics Data Frame Source – “Player Statistics” Sheet of nba_data_2019_2020.xlsx
*	NBA Player Salaries Data Frame Source – “Salaries” Sheet of nba_data_2019_2020.xlsx
*	NBA Team Statistics Data Frame Source – “Team Statistics” Sheet of nba_data_2019_2020.xlsx

## Data Sources
For my project, I will collect three data sets from [Basketball Reference](https://www.basketball-reference.com/):

1.	The Player Statistics data set presents information and performance statistics about each player (514 in total) such as their position (Pos), team (Tm), games played (G), minutes played (MP), field goal percentage (FGp), 3-pointers per game (P3), 3-point percentage (P3p), effective field goal percentage (eFGp), free throws per game (FT), free throw attempts per game (FTA), free throw percentage (FTp), offensive rebounds per game (ORB), defensive rebounds per game (DRB), total rebounds per game (TRB), assists per game (AST), turnovers per game (TOV), points per game (PTS), true shooting percentage (TSp), 3-point attempt rate (P3Ar), defensive win shares (DWS), and defensive box plus/minus (DBPM).
*	Effective field goal percentage (eFGp) is the percentage of field goals a player makes and adjusts for the fact that a 3-point field goal is worth one more point than a 2-point field goal.
*	True shooting percentage (TSp) measures shooting efficiency that takes into account field goals, 3-point field goals, and free throws.
*	3-point attempt rate (P3Ar) is the percentage of field goal attempts from 3-point range.
*	Defensive win shares (DWS) estimates the number of wins contributed by a player due to his defense.
*	Defensive box plus/minus (DBPM) estimates a player’s defensive contribution to the team when that player is on the court.
2.	The Player Salaries data set presents the salaries of all (520) NBA players for the 2019-2020 to 2023-2024 season.
3.	The Team Statistics data set presents performance statistics about each of the 30 NBA teams such as their win-loss percentage (WLp), field goal percentage (FGp), 3-pointers per game (P3), 3-point percentage (P3p), free throws per game (FT), free-throw attempts per game (FTA), free throw percentage (FTp), offensive rebounds per game (ORB), defensive rebounds per game (DRB), total rebounds per game (TRB), assists per game (AST), turnovers per game (TOV), points per game (PTS), 3-point attempt rate (P3Ar), pace, true shooting percentage (TSp), effective field goal percentage (eFGp), offensive rating (ORtg), and defensive rating (DRtg).
*	Win-loss percentage (WLp) is the percentage of games a team wins. I decided to use this statistic rather than simply using wins to quantify winning because some teams played more games than others prior to the COVID-19 play stoppage.
*	Offensive rating (ORtg) shows how many points a team scores per 100 possessions.
*	Defensive rating (DRtg) shows how many points a team allows per 100 possessions.


## Power BI Project Dashboards
![Correlations](https://github.com/xavier-lim/basketize/blob/master/images/correlations.PNG)

![Payroll](https://github.com/xavier-lim/basketize/blob/master/images/payroll.PNG)

![Raptors](https://github.com/xavier-lim/basketize/blob/master/images/raptors.PNG)

## Conclusion
In conclusion, winning teams tend to score a lot of points, play good defense, rebound the ball well, and shoot efficiently. The Basketize model takes all of these factors into account when optimizing a roster. NBA teams can use this model not only to determine who they should target in free agency, but also to determine which players they should trade away/for to improve their team's statistics. In addition, this model can be tailored to a team's needs and style of play. According to the model, the free agents the Toronto Raptors should target are Christian Wood, Dwight Howard, Fred Vanvleet and Meyers Leonard. Interestingly, Vanvleet plays for the Raptors so the model is essentially suggesting that the team should resign him.

## Acknowledgements
* Holly Wiberg, PhD Candidate at MIT Operations Research Center, presented a workshop at the 2020 MIT Sloan Sports Analytics Conference (SSAC) about optimizing rosters.
  * [Github Repo](https://github.com/hwiberg/SSAC2020)
  * [SSAC20: An Optimization Approach to Roster Creation](https://www.youtube.com/watch?v=_eBk1bSjDs8)

## Author

* **Xavier Lim** - [LinkedIn](https://www.linkedin.com/in/xavier-lim14/) | [Portfolio Website]( https://xavier-lim.github.io/)

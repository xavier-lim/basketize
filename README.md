# Basketize
Basketize is an optimization model whose main objective is to minimize an NBA team's salary while achieving key team statistics likely to lead to wins. It uses an exploratory data analysis (EDA) and mixed-integer optimization (MIO) to determine which combination of 12 players will collectively lead the NBA in all team statistics likely to lead to wins. The model is also used to determine which free agent players the Toronto Raptors should target in the 2020 offseason to maximize their chance of winning.

## System Requirements
* Julia
*	NBA Player Statistics Data Frame Source – “Player Statistics” Sheet of nba_data_2019_2020.xlsx
*	NBA Player Salaries Data Frame Source – “Salaries” Sheet of nba_data_2019_2020.xlsx
*	NBA Team Statistics Data Frame Source – “Team Statistics” Sheet of nba_data_2019_2020.xlsx

## How to Run the Code
1.	[Download Julia](https://julialang.org/downloads/) 
2.	Download/clone this repo
3.	Open Julia and insert the following lines of code
      ```
     julia> using IJulia()
      julia> notebook()
      ```
4.	After Jupyter local host browser opens, select the folder with the downloaded/cloned repo 
5.	Run Basketize.ipynb

## Acknowledgements
* Holly Wiberg, PhD Candidate at MIT Operations Research Center, presented a workshop at the 2020 MIT Sloan Sports Analytics Conference (SSAC) about optimizing rosters.
  * [Github Repo](https://github.com/hwiberg/SSAC2020)
  * [SSAC20: An Optimization Approach to Roster Creation](https://www.youtube.com/watch?v=_eBk1bSjDs8)

## Author

* **Xavier Lim** - [LinkedIn](https://www.linkedin.com/in/xavier-lim14/) | [Portfolio Website]( https://xavier-lim.github.io/)

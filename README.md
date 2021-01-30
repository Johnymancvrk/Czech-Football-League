# Data Processing in Python Project - Czech Football Fortuna League Analysis
Authors: Jan Cvrček, Jan Stuchlík

## Aim of the project
The aim of our project is to analyze various data about teams and players in the Czech Football Fortuna League, visualize the outputs of the analysis and predict results of future matches based on historical data, all using Python. Our data was obtained from https://fbref.com/en/comps/66/Czech-First-League-Stats. The process of obtaining the data as well as the analysis is described by the following diagram.

![Flowcahrt](https://user-images.githubusercontent.com/72010018/106131351-dd27e280-6162-11eb-9359-ede9e7b28116.jpg)

## Description of all steps:
1. We scraped the website above to get dataframes with statistics on players, teams, and scores. The code and outputs for this part of the project can be found in these files: Players_Stats_Scraper.ipynb, Teams_Table&Scores_Scraper.ipynb.

2. The data was cleaned so that we could use it for meaningful computations. Data cleaning and analysis with comments can be found in these files: Players_Cleaning&Analysis.ipynb, Teams_Cleaning&Analysis.ipynb. The nice dataframes were written into csv files to be accessible in other notebooks. They are available in these files: Final_Player_Stats.csv, scores_clean.csv.

3. We analyzed statistics on players and teams, and visualized the results in tables and graphs.

4. We wrote a function that predicts the results of future games based on historical data (head-to-head games, current form, league table rank, home/away team). The function and predictions can be found in Predict_function.ipynb.

5. We also scraped data about players' market values (from https://www.transfermarkt.com/ in Market Values.ipynb) and nations' ranking (from https://www.fifa.com/fifa-world-ranking/ranking-table/men/). We merged the data with players' statistics and ran a linear regression to estimate the effect of different players' characteristics on their market value. The regression with preparation and results can be found in Merging and OLS.ipynb.

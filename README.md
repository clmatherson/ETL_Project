# ETL_Project
ETL Group Project 

<h2 align="center">:dollar: :soccer: Major League Soccer and Salary :soccer: :dollar:</h2>

# E: Extract 
https://fbref.com/en/comps/22/1558/stats/2017-Major-League-Soccer-Stats#all_stats_standard
https://www.kaggle.com/crawford/us-major-league-soccer-salaries?select=mls-salaries-2017.csv

Downloaded the data from the csv files to a Jupyter Notebook


# T: Transform
cleaned the data:
    took out the '-' from players names in the fbref table - this allows the two tables to sync up
Kept the duplicate players - they played on multiple teams (trades)


# L: Load
Loaded the newly transformed data and tables into postqresql 
Postqresql was chosen because it allows for easier manipulation of the tables.  Anyone wanting to determine how much a player makes per min the play can easily perferm that function, they can also determine how much a squad pays it players and which squad pays the most or the least. 


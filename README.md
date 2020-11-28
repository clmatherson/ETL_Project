# ETL_Project

<h2 align="center">:dollar: :soccer: Major League Soccer and Salary :soccer: :dollar:</h2>

Contributers: Craig Matherson, Paul Eppers, Juliann Pezzullo, and Connor Lanier

# E: Extract 
*https://fbref.com/en/comps/22/1558/stats/2017-Major-League-Soccer-Stats#all_stats_standard

*https://www.kaggle.com/crawford/us-major-league-soccer-salaries?select=mls-salaries-2017.csv

Downloaded the data from the csv files to Jupyter Notebook
*    Included header = 5 for the 2017 Major League Stats so the data would be starting with the correct headers and would not have to lose drop the top rows


# T: Transform
Cleaned the fbref data:
-    Renamed columns to make column headers clearer
-    Cleaned up the player column by taking out the '\', the duplicate name, and '-'; allowing for two tables to sync and coorespond with the player names
-    Split the nation column into two additional columns named nation_2-two digit code and nation_3-three digit country code
-    Changed the column types from object to integer or float where needed

Cleaned the salaries data:
-    Renamed columns
-    Dropped unnecessary columns (repeated from fbref table)
-    Kept the duplicate players - they played on multiple teams and had different salaries for the teams
    
Created new tables from fbref data allowing for smaller tables; users can choose to pull in the additional information based on their needs 
    


# L: Load
add image of relationship diagram

Loaded the newly transformed data and tables into postqresql 

Postqresql was chosen because it allows for easier manipulation of the tables.  Anyone wanting to determine how much a player makes per min the play can easily perferm that function, they can also determine how much a squad pays it players and which squad pays the most or the least. 


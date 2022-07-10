#Election Analysis
								
#Project Overview:

This is an elections audit analysis done on behalf of the Colorado Board of Elections. Following tasks needed to be completed to project the winner.
•	Total number of votes 
•	A total list of county votes
•	Percentages and total votes each county received
•	Winning county based on votes and rate
•	A list of candidates who ran for the election
•	Percentages and total votes each candidate received 
•	The winner of the election based on rate and votes

#Summary:

The analysis of the election shows that:

![](https://github.com/smzd/Election_Analysis-/blob/main/Resources/election_analysis_terminal.png)
Fig: Analysis Output on the Command Line

•	There were 369,711 votes cast in the election

•	The candidate who ran for the election were:
Charles Casper Stockham, 
Diana DeGette, 
Raymon Anthony Doane.

•	3 Counties total number of votes and percentage of total votes: 
Jefferson: 38,855 & 10.5%,
Denver: 306,055 & 82.8%,
Arapahoe: 24,801 & 6.7% 

•	County Denver had the most significant number of votes: 306,055 and an 82.8% winning rate.

•	Number of votes and percentage of votes each candidate got were:
Charles Casper Stockham: 23.0% (85,213), 
Diana DeGette: 73.8% (272,892), 
Raymon Anthony Doane: 3.1% (11,606).

•	Diana DeGette won the election. Her vote count was 272,892, and her percentage of the total vote was 73.8%.

#Election-Audit Summary:
							  								
In this analysis, we assist Tom in the Colorado board of election by helping him with the election audit. We are providing the proposal on how the election committee can use this program for any election with some modifications. 

•	This program is a robust script for doing any election analysis. We take the .csv file open, read and write it in a text file with the help of different libraries such as CSV and OS library. To use this program in further analysis, we make changes to the file_to_open and file_to_load paths to our desired path.

![](https://github.com/smzd/Election_Analysis-/blob/main/Resources/election_file_path.png)
Fig:Changing File Path

We can use this file for any election analysis calculations, and it can be used for county/state/federal election analysis. All we need to do is change the county variables to the desired variable to match the research. In the File_to_load, we are using the .txt extension to write our file. We can change the print instruction to our desired need.

•	Next, we should check for missing data values or corrupted strings of rows. This is very important since the corrupt value will give false results. We can use the following line to get rid of the null values. 

![](https://github.com/smzd/Election_Analysis-/blob/main/Resources/election_null_value.png)
Fig: Getting Rid of Null Values

We can import pandas and use isnull().sum() changing method and dropna() to eliminate the null values.

•	We can also ask for user input on election analysis to make the program interactive. We need to have multiple election data in the resources folder. So when users would like to display a specific year on the analysis study. They put an input for the year they want to show the election analysis; we can have an IF conditional saying that if the user input string is the desired number we are looking for, it corresponds to a file. That file name gets transferred as a string on the file_to_load variables. Or else error no year found.

#Resources:

Data Source: election_results.csv

Software: Python 3.9.7, Visual Studio Code, Version: 1.68.1 (Universal)

https://stackoverflow.com/questions/7894856/line-contains-null-byte-in-csv-reader-python


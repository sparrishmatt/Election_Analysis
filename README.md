# Election Analysis

## Analysis Overview
The purpose of this analysis was to use python to pull information from a csv file containing the votes for an election. Code was written to tally the total number of votes, find the winning candidate, and find what counties the majority of the votes in the election came from. 

To finish the project, the final goal was to take all of the data that had been analyzed from the csv file and write that information to a text file containing only the information about the vote percentages and totals. 

## Election Audit Results
In order to analyze the results of the election, a few questions must be answered and parts of the code must be reviewed.

---

* How many votes were cast in this congressional election? 
<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/total_votes.png" height="150">

For the precinct having its election results reviewed there was a total of 369,711 votes. The code to find this vote total was a total_votes variable initialized at zero that has one vote added to it for every row in the csv file. 

<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/vote_counter1.png" height="150">
<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/vote_counter2.png" height="150">

---

* Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.

<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/county_results.png" height="150">

There are three counties in the precinct being audited: Jefferson, Denver, and Arapahoe. Jefferson county was the source of 10.5% of the votes, which comes out to 38,855. 82.8% of the votes come from Denver county, which is 306,055 votes. The final 6.7% of the vote came from Arapahoe county which is 24,801 votes.

This information was found by creating an empty list of counties and an empty county votes dictionary in python. The names of the counties are pulled from the csv file, and then every time that county appears one vote is added to the county votes. 

<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/county1.png" height="150">
<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/county2.png" height="180">

---

* Which county had the largest number of votes?

As can be seen in the question above, a large majority of the votes cast in this election came from Denver county. The code used to present the winning county, as well as the code that writes the county results to our text file can be seen below. 

<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/county3.png" height="200">

---

* Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.

<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/candidate_results.png" height="150">

Three candidates were running in this election and they will be presented in order of the least votes received to the most votes received. Raymon Anthony Doane received 3.1% of the vote which was only 11,606 votes. The second candidate is Charles Casper Stockham with 23.0% or 85,213 votes. Finally, the candidate with the most votes received was Diana DeGette with 73.8% or 272,892 votes. 

The code used for this section is very similar to the code used to find the county results. The main difference just being the variable and list names.

<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/county1.png" height="170">
<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/candidate1.png" height="180">

---

* Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

Once again the candidate that received the most votes was Diana Degette with 73.8%/272,892 votes. The code used to find the "winning candidate" is very similar again to the code used to find the county where the most votes came from. 

<img src="https://github.com/sparrishmatt/Election_Analysis/blob/main/Resources/county3.png" height="230">

## Election Summary
The code used to perform this election analysis could be used to perform a similar analysis for any election results presented in the same format. For other formats (like candidate information being listed in different columns), elements of the code could be quickly changed in order to work with that information. If more information was given for each vote that the audience of the report would be interested in, then it would be easy to initialize new variables and write a few more lines of code that would also output the results of that information. If a person wanted to make these changes and  understands how the code is working (the code is commented so this should not be a problem), then it should be easy enough for them to accomplish.

### Relief Pitcher Prediction Model 

* **Data used**

	The Situational_Pitching directory contains FanGraphs relief pitcher data from 2015 through 2023

 	Data is split up across innings, number of outs, and the amount of runners on base

* **How it works**

  	First, a late game situation is generated, such as: 7th inning, 1 out, runners in scoring position

  	To determine which pitcher would be best suited for any given scenario, I created a custom 'Effectiveness' statistic

   	'Effectiveness' is built with a combination of different stats such as OBP, WHIP, FIP, K-BB%, etc.

   	Depending on the severity of the late game situation, each stat used to calculate a relief pitcher's effectiveness is weighted differently in terms of importance

   	Once all relevant stats are weighted and the effectiveness statistic is calculated, a Random Forest Regressor is utilized to make the final prediction


### Matchup History Analysis (WIP)

* **Data used**

   	All matchup history between all currently active MLB pitchers and all currently active MLB hitters was scraped from BaseballSavant's website

* **How it works**

   	This is still a work in progress, but I plan to generate a more realistic game like situation where, in addition to the inning, outs, and runners on base, 3 hitters from the same team will be chosen to simulate who the pitcher, at minimum, must face
  
   	By using their matchup history I can make a more informed prediction on what relief pitcher would be most effective
  
	

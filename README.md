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

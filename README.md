# CommuteChaos
UCB Bootcamp Project

For chart pictures and map pictures, please install this extension first before run the code.
pip install geopy
Also You must run this in your Terminal jupyter nbextension enable --py gmaps


Commute Chaos Project
Major Findings
January 14th, 2020

By:  The Data Ninjas (Kat Anggasastra, Sreeteja Bollepalli, Molly Cox, Melissa Wright)

Research Questions:
 How does today’s commute compare to the same route 5 years ago?  Everyone on our team has experienced sitting in traffic either going to or coming from work, or to/from class.  Has it always been this way?
We looked at several online databases, but couldn’t find a free one with an api and historical data:  PEMS (Caltrans highway data) - has historical highway speed info but no point to point commute durations.
Google Directions API - doesn’t have historical data, but can give you a prediction of commute time based on their data/algorithms.
TomTom API - charges a fee for using their data, so we didn’t pursue it
MapQuest - Does not store historical data.

Conclusion:  We couldn’t get historical data for a complete route, so we opted to change our question.

What does the commute look like in the Bay Area from various locations?
Initially, we each used google maps to find how long each of our commutes were projected to take.  In the Google Maps API, you can specify either “Depart At” or “Arrive By” times.  When we changed the departure times, we found that the commute duration varied quite a bit.  So we decided to explore commute start time for each day of the week. Since the Google Directions API only lets you enter today’s or future dates, we chose the first week in March to explore, as there are no holidays that week.

Conclusion:  The commute with the most variation of our 4 commutes was the Moffett Field to San Francisco commute, so we focused on this one for our data analysis.

How does the commute duration change day to day?
We created 2 charts showing average commute time to and from work to answer this question:



Conclusion:  If you want to have the shortest commute times, weekends for this commute are better on average than other days. At this level of detail, you’d want to plan for at least an hour in the car.

How does the commute duration change based on departure time?
We created bar charts for each day of the week, one bar for each hour, to see how the commute varied day to day (similar to the bar graphs above).  We also created a table with commute times, where you can see the best and worst times to depart for a given commute.



Conclusion:  Leaving for work at 5AM, you have the shortest commute time, while leaving at 8AM increased your time in the car by 30 minutes or more.  Coming home, either leaving early or staying until 7PM would reduce your commute time some days by 30 minutes.

How does the commute change depending on direction (morning to work, evening to home)?
Leaving earlier in the morning produced the shortest commute time.  By the afternoon, most commutes increased by several minutes to as much as 30 minutes. (See chart above for comparison)
So, in general, the shortest commute home was greater than the shortest commute to work.


To view our presentation, go to: Commute Chaos






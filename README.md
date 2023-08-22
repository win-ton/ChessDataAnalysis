# ChessDataAnalysis
A in depth analysis of Chess Data from lichess.org. 
This project looks to answer 4 seperate questions:

1. Rating difference versus win likelihood
First, by subtracting our higher-ranked player’s rating from the lower-ranked player we can find the difference between the ratings
Second, we take into account the winner of the said game (White or Black).
Third, we graph these values using most likely a line graph where our y-axis is the percentage chance they win the match and our x-axis would be the difference in rating
If there is a generalized pattern, then we can find the linear regression of difference in rating by win likelihood

2. Combined Rating versus length of a match
First, we add the rating of both players together getting the “total skill” of the match.
Second, we pull the value of total time in each of these games (by subtracting the starting time of the match by the ending time of the match.
Third, we graph the values against each other either by grouping the rating in groups of hundred or by graphing them on a line graph. Then we observe the length of the game and if there is a generalized pattern we can find the regression between the values by running a statistical test such as linear regression.

3. Likelihood of a given color winning a match as rating increases
In this question, we have to again find the sum of the rating of both players as our first step
Following this, we need to group the rating into groups so that we can examine the groups in more detail (parse rating groups by 100’s)
After this, we want to find the percentage of white wins, black wins, and draws as the combined rating goes up.
Finally, if a trend is observed we can run a regression analysis (Random Forrest) on the data to see if there is a more generalized trend and the exact value of the said trend.

4. Type of victory at different rating chunks
Similar to the last two questions we want to find the combined rating of both players.
Then, parse them by their rating groups
Finally, we can run the chunks by their percentage of wins by resigning, mate, or timeout
This can be represented by multiple pie charts showing the distribution of the 3 possible values amongst different skill groups.
Finally, we can observe the increase in a certain style of victory as the rating goes up or down.

5. Notes:
When trying to get our data to be precise we will have to use clustering to get matches that are in close proximity to each other normally by group combined ratings together. What this allows us to do is examine data in matches where players are equally skilled
In data where we want to find the difference between the rating of two players what we are particularly interested in is seeing if the more massive difference in player skills leads to a decrease in moves made, time spent in the match, and an increase in victories. To do this we can use classification by predetermining the differences between the players and grouping them together.


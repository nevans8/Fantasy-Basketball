# Fantasy-Basketball
Values fantasy basketball players by calculating the marginal probability of winning matchups

Uses basketball reference to download players stats.
Calculates each team's predicted totals in each of the 9 categories by summing over all the players on a team. 
Compares distributions to calculate the probability that I'd win each category against all other teams.
Calculates overall probability that I win a matchup.
Adds each player to the team and recalculates the probability of winning the matchups.
The player's value is the marginal probability of winning matchups.

Field goal and free throw percentage was tougher than the others assists/ blocks/ points/ etc. 
For categories such as blocks I could just calculate totals, but for fg and ft its percentages.
I had players' mean and sd of shot attempts and shots made, so I would add up all shot attempts and shots made.
But how do you calculate the sd of the fg percentage = shots made / shots attempts. 
I estimated a standard deviation decrease in the percent would be 1/2 a sd decrease in shots made and 1/2 sd increase in the attemps.
This isn't perfect, but I haven't taken enough math stats to do better.

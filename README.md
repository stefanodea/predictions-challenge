# Predictions Challenge

# Intro

Being stuck in the house due to COVID-19 and without any (or very few) basketball games, 
we thought it might be fun to share some of our data we use in https://newstats.eu and challenge you to give your
predictions on historical data.

# Dataset Description
We anonymized and uploaded data from the first 5 rounds of 3 different leagues in the corresponding directories.
- [league1](league1)
- [league2](league2)
- [league3](league3)

In each of these folders you will find 2 files:
- **train.csv** : ([example](league1/train.csv))

It contains the data for the first 5 rounds of the anonymized league.
Every pair of rows refers to a single game in that round. As an example:

```
ROUND,GAME,TEAM,HOME,2P,2PA,3PA,3P,FT,FTA,ORB,DRB,AST,TOV,STL,PTS
1,game_1,team_10,1,19,34,20,7,7,16,9,23,12,23,4,66
1,game_1,team_2,0,21,40,22,10,9,11,8,24,18,16,13,81
```

In round 1, in game_1, the home team(home=1) was team_10 and away team(home=0) was team_2. The final score was 66-81.
The rest of the fields are obvious. The anonymized versions of the teams are only valid within the same league (e.g the team_2 
of league1 is not the same team with team_2 of league_2).

- **test.csv** : ([example](league1/test.csv))

This is the file you need to fill out the last column.
This entry:
```
ROUND,GAME,TEAM,HOME,PTS
6,game_30,team_4,1,
6,game_30,team_3,0,
```
indicates that in round 6 the home team team_4 plays versus team_3. You will need to fill out the predicted points for each team.

# Participation

In order for you to participate, just clone the current repo the fill out the *test.csv* files in the leagues directories.
We will rank the submissions on 2 categories:
- Winners prediction (i.e accuracy in predicting the winner in each game)
- Total points in game (i.e accuracy in predicting how many points will be scored in total in each game)

We will publish the winners and you will get a chance to present your approach.
You might have questions, comments, so feel free to reach out on our twitter https://twitter.com/NewstatsEu

***Deadline: 29 March (tentative)***

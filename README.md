# Introduction 
I have always followed football, but I have never been much of a fan of fantasy sports, especially Fantasy Premier League. There's so much uncertainty, the sesason is arduously long, and my luck has never been that good. However, this season (20/21) my friends convinced my to give it a try. I ended up waiting until the last minute to create my team and simply threw together some player that I thought would have success. My hopes weren't very high but somehow as 2020 came to an end I was within striking distance of the top of the table. At almost half way through the season I was looking to use my wild card, and I thought some data modeling and optimization could improve my chances of creating the best team.

The prospect of having a chance at winning lead me to an FPL API (https://fantasy.premierleague.com/api/bootstrap-static) and ecouraged me to explore the data and write a bit of code.

# EDA
After creating my dataframes and cleaning up the data, I decided to draw out some basic patterns. For example looking at the relationship between the in-game price of a player and their total point production in the season so far.

![alt text](https://github.com/alexanderd14/FPL-Optimization/blob/main/fpl.png)

This is great for identifying bargain players line Son, Bamford and, Bednareck, who are all earning for more points than their prices suggest. However, I wanted to get the most out of my team not just a few bargains.

# Modeling 
I am still in the process of predicting scores for the the rest of the season using Dataiku for ease of feature engineering and model training speed.

# Optimization
Once I have good and viable predictions I will run them through my optimization function which finds the maximum number of point I can recieve with the dollar amount alotted in FPL. The code is annoted step by step. This is the output without modelled predictions for team optimization of the players who have scored the most so far this season. 

![alt text](https://github.com/alexanderd14/FPL-Optimization/blob/main/fpl2.png)

The linear optimization also accounts for the formation desired by the user.

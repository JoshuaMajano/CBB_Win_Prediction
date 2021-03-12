# CBB_Win_Prediction

Included in repo:
  1) Kaggle dataset
  2) Jupyter notebook with analysis
  3) Powerpoint slides of presentation


Link to presentation: https://youtu.be/5k9ES-vE-hc

I am Joshua Majano, a student in the Master's of Data Science program at the Univeristy of San Francisco and I was curious about how possible it is to predict the number of wins for a Division I College Basketball team using only their stat numbers for the season.

The data itself comes from Kaggle and is included in this repository. It includes data from ~353 teams spanning the 2015-2019 seasons with 24 columns that include the team stats for the season as well school name, conference they play in, and their seeding for the postseason. For this project, I only considered the columns that had the team stats, and not the school name, conference, or anything that could be related to the postseason as not every team had data for the postseason or their seeding. For as much as data is now an instrumental part of sports, I wanted to test how accurate of a win prediction we can get from just the team stats without knowing the school or if they made the postseason. Also, considering all of the different stats out there, I was also curious to see if we can highlight any specific features that stand out and might have the most predictive power to win prediction.

With so many features, how would we find out which ones to use?
I broke this question down to 3 sub categories of the data. One was just using all of the 16 features that corresponded to the team stats. Second was using 8 features of the data that corresponded to what Dean Oliver deems as the "Four Factors of Basketball Success" which boils down to score on every possession, pick up all rebounds, get to the free throw line, and protect the ball. Lastly, I considered using the adjusted efficiency stats which are mixture of team's offensive and defensive stats, and their pacing of the game.

From fitting many regression models with different hyperparameters that could affect what each model would deem important among the features, the best model overall came from fitting a Ridge regression model using all of the features which had a mean absolute error of about 1.93, or in other words, win predictions were off by just under 2 wins, which is pretty respectable. This does highlight how all possible features were needed to get our best predictions and reminded me that the numbers alone cannot tell the full story in sports. But it was still impressive to see how much of the win story for each team the data was able to provide and that perhaps with more features from the dataset or features outside of the dataset, we can get a more accurate win prediction.

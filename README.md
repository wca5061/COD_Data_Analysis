# COD_Data_Analysis

This project analyzes data from a Call of Duty game dataset, focusing on several variables that describe the player's performance, the type of experience boosts received, the outcome of matches, and the opponent's score. Below is an overview of the tasks performed and their results:

# 1. Exploring the XPType Variable (Categorical Analysis):
The XPType variable represents the type of experience boost the player receives during matches. Two types of XP boosts are observed: "10% Boost" and "Double XP + 10%". The dataset shows that the "10% Boost" is more frequent, occurring in 61.1% of matches, while "Double XP + 10%" occurs in 38.9%. There are no missing values for this variable, ensuring the data's completeness.

A bar plot of the XPType distribution shows that "10% Boost" is much more common than "Double XP + 10%", suggesting that the player is more likely to encounter or select the "10% Boost" XP type. The analysis is further supported by the absence of missing values, making the insights reliable.

# 2. Match Outcomes (Wins, Losses, and Draws):
The Result variable was used to determine the outcome of the matches. The player's team score was compared to the opponent's score to classify each match as a win, loss, or draw. The dataset reveals that the player's team won 54.03% of the matches, lost 44.55%, and tied 1.42%. The analysis indicates that the player's team had a positive win rate, with more than half of the matches being wins.

A bar plot and a pie chart were created to visualize the distribution of wins, losses, and draws. Both visualizations confirm that wins are the most frequent outcome, but the relatively high percentage of losses highlights areas for improvement.

# 3. Inference Using Logistic Regression:
A logistic regression model was created to investigate the effect of the opponent's score on the probability of the player's team winning. The binary response variable Win (1 for a win, 0 for a loss or draw) was modeled against the opponent's score as the predictor.

The logistic regression model’s results showed a negative relationship between the opponent's score and the probability of the player's team winning. Specifically, the coefficient for opponent_score was -0.07224, which implies that for each additional point scored by the opponent, the odds of the player's team winning decrease by approximately 7%. The model suggests that the player's team is less likely to win as the opponent's score increases, which is expected since the opponent's score is a direct measure of their performance.

# Conclusion:
This project provided insights into the player's match outcomes, XP boost types, and the impact of the opponent’s score on the player's team’s performance. The player's team has a positive win rate, with more than half of the matches being victories. The "10% Boost" XP type is the most frequent, suggesting that it is a common or easily accessible boost. The logistic regression model confirmed that the opponent's score negatively affects the player's team’s probability of winning. These insights can inform strategies for future gameplay and improvement.

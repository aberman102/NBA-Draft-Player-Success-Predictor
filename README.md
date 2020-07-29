# NCAA Player Prediction Project

As the sports world continues to grow and devlop, there has been a movement for teams to start building their rosters through the amateur draft. Drafting young players is considered advantageus due to the incredibly low salarys paid out to young players and the ability to hold onto a player for a long period of time due to league negotiating restrictions. While building through the draft has a very high upside, there is also the downside. Team's must take educated guesses on the players they are drafting and hope that the players they pick are going to be successful in the league. In the National Basketball Association (NBA), teams get two picks per draft and the average career length is 5 years. What this tells us is that most organizations are struggling to pick the right rookies to improve their rosters. I have set out to find a better way to scout rookies based on their NCAA production. I believe, that being able to predict off of statistical output provides for a better scouting report than just using the "eye test".

## The Approach

1) Scrape NBA final statistics, Awards and bio as well as NCAA production (https://www.sports-reference.com/)

2) Engineer advanced statistics to give deeper insight into player performance

3) Build and test models on data

4) Review confusion matrix to view gaps in the model

## The Model

I started by splitting the data into training and test sets. Next, I tested multiple models and used both the accuracy and f1_Macro metric to judge the abilities of our model. The models I tested were Logistic Regression, KNN, a Decision Tree, Random Forest, a Voting Classifier, and an XG-Boost. I found that XG-Boost produced the best results on the test set. The model's accuracy score was 96.73% and an F1 score of 71.63%. I found that the model was able to predict draft busts, veterans and All-Stars at 100% but when it came to All-Pro players and Hall of Famer's the model's predictions dropped down to 50%. The fact that the model was able to predict the first three classes so well was amazing, I'm not as worried about the model's "struggle" to predict All-Pro players and Hall of Famers as 50% accuracy on both classes is still an outstanding achievement.

## Future of the Project

1) Our model is currently built off of the draft classes between 1985 and 2000, we still dont know if it continues it's predictive strength after the year 2000.

2) Extend prediction's to players who are outside the NCAA, am I able to create a model that can predict the success of international prospects?

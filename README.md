****NFL ANALYSIS****

Team Members: Sean Oberer, Vatsal Rathod, Piyush Jain, Garrison Bolick, Anuj Sharma

**Introduction to Problem:**

For our project, we want to predict what a NFL running backs fantasy football production will be based on their statistics from 2018. Fantasy football is an extremely popular game where people can own virtual teams with NFL players in a privately owned or public league with other real people that also pick their teams. We want to predict what a running backs production would be specifically because running backs are the most valuable players in the majority of fantasy football leagues and consistently provide the most points for fantasy football owners. We will be taking their fantasy football production statistics from 2018 and try to predict what their future fantasy production will be the upcoming season. 

**Research Questions:**

What will a NFL running back's fantasy football point per game production be based on their in-game statistics such as rushing/passing yards per game, touchdowns per game, etc.? 

What in-game statistics contribute most consistently to a NFL running back's fantasy football point and point per per game production?

How accurately does a NFL running back's previous season statistics predict what they are going to do the next year they play? 

It will help us to predict and analyse:
NFL running back analysis
To predict the outcomes an NFL running backs fantasy football productions based on receiving yards, rushing yards, touchdowns, etc.


**Data Resource:**

[Fantasy Pros] (https://www.fantasypros.com/) Relative attributes that we are interested in using from the data for our project: Position: Running Back, stats: ruhshing yards per game, rushing attempts per game(the time in which the running back carries the football), and touchdowns per game.


**Future Work:**

Following are the list of topics which if given an opportunity in future we might able to work on:
NFL running backs previous fantasy football season production
Heat map of rushing yards, receiving yards, etc. in relation to fantasy points
Pairplot to see where there is a stronger relationship for some variables such as rushing yards, touchdowns, etc. as opposed to others

**Domain Knowledge**

Two of our group members - Sean Oberer and Garrison Bolick, have been playing fantasy football for and know the ins and outs of how everything works with fantasy football. Although sports is mostly opinionated, running backs have the second highest point differential and score the most total points out of any other position in fantasy football (Orriss et al., 2021). Because of this, we wanted to focus on NFL running back given the time constraints since they have the most impact on the success of a fantasy football team.


**Data Preparation**

When we first started our project, we originally were going to try to predict what a NFL running back's total fantasy football point production would be. However, due to the violent nature and human aspect of the sport - we decided it would be best to predict what a running back's fantasy football point per game production will be since this will most accurately predict their true fantasy football point production while taking into account games players may miss due to injuries, illnesses, personal matters, etc.. Because we changed our dependent variable to be fantasy points per game, we also had to change the unit of measure for our original independent variables (total passing yards, total touchdowns, total rushing yards, etc.) to total passing yards per game, total touchdowns per game, total rushing yards per game, etc. so that we can accurately predict what a running back's fantasy football production will be when they are on the field. 

Data Understanding and Exploration

<img width="159" alt="Screen Shot 2021-11-13 at 3 37 01 PM" src="https://user-images.githubusercontent.com/59974878/141658337-c6159e01-72cf-4e88-9c3e-80335c1504e7.png">

<img width="158" alt="Screen Shot 2021-11-13 at 3 38 20 PM" src="https://user-images.githubusercontent.com/59974878/141658389-d6d3aac4-f554-4eab-91d7-39b41c5c8ea9.png">

Based on our pairplot above, we found that the in-game statistics such as passing yards per game, rushing yards per game, touchdowns per game, etc. were all linearly correlated with our dependent variable fantasy points per game. 

<img width="627" alt="Screen Shot 2021-11-13 at 3 39 38 PM" src="https://user-images.githubusercontent.com/59974878/141658436-7bd6417f-cabe-44b5-a4d9-70ba64eb5c62.png">

We created a heat map above to see how much of a correlation there was specifically between all of our independent variables (passing yards per game, rushing yards per game, touchdowns per game, etc.) with fantasy points per game. Based on our heat map, we found that rushing yards per game, rushing attempts per game, attempts per game, targets per game, and total touchdowns per game have the most impact on our dependent variables fantasy points per game. Rushing touchdowns per game also had a heavy impact on a NFL running backs fantasy football points per game but we decided to combine both rushing touchdowns per game and passing yards per game since total touchdowns per game will be more of an accurate indicator for how many touchdowns that particular running back will produce. 

**Machine Learning (Modeling)**

For our project, we decided to use three different machine learning models: linear regression, random forest, and bagging ensemble. The reason we chose linear regression was because of the high correlation between a NFL running back's game stats such as passing yards per game, rushing yards per game, touchdowns per game, etc. and their fantasy points per game. After running our linear regression model, we ran into some overfitting problems which we will discuss in the evaluation. After running into our overfitting problems, we wanted to create a couple of ensemble models because of their good predictive performance. 

**Evaluation**

Based on our R squared values, our linear regression model for predicting FPTS/G was the most accurate with 99.97% of our data fitting the regression line. As a result of our extremely high R squared value, our model was extremely accurate with our data but wasn't the best for predicting an NFL running back's fantasy football point per game production for future seasons since the predictions were so close to the data set we had. We also ran into another problem with being able to identify who the predicted points per game was associated with like we intended to when we first began our project. As a result of this, our predictions are rather limited in how helpful they can be for someone who plays fantasy football unless they have the data that we used so that they can go back and search for the player using their Rank column from our data that is displayed with our predictions. Our random forest model had an R squared value of .9394 meaning that 93.94% of the data fit the regression line and our ensemble bagging model had an R squared value of .9175 meaning that 91.75% of our dataset fit the regression line. Because of the overfitting issues, the predictions from our random forest and bagging ensemble models might be best to use for predicting what a NFL running back's fantasy football points per game will be based on their previous season's statistics.


**Conclusion**


**References**

Orriss, J., Planas-Arteaga, S., Yen, P., &amp; Worthy, C. (2021, June 5). The importance of running backs in fantasy football. CROW WORTHY. Retrieved December 8, 2021, from https://www.crowworthy.com/posts/the-importance-of-running-backs-in-fantasy-football/. 



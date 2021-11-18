****NFL ANALYSIS****

Team Members: Sean Oberer, Vatsal Rathod, Piyush Jain, Garrison Bolick, Anuj Sharma

**Introduction to Problem:**
For our project, we want to predict what a NFL running backs fantasy football production will be based on their statistics from previous years. Fantasy football is an extremely popular game where people can own virtual teams with NFL players in a privately owned or public league with other real people that also pick their teams. We want to predict what a running backs production would be specifically because running backs are the most valuable players in fantasy football leagues and consistently provide the most points for fantasy football owners. We will be taking their fantasy football production statistics from previous years and try to predict what their future fantasy production will be the upcoming season. 

**Research Questions:**
What will a NFL running back's fantasy football point per game production be based on their in-game statistics such as rushing/passing yards per game, touchdowns per game, etc.? 

What in-game statistics contribute most consistently to a NFL running back's fantasy football point per game production?

How accurately does a NFL running back's previous season statistics predict what they are going to do the next year they play? 

It will help us to predict and analyse:
NFL running back analysis
To predict the outcomes an NFL running backs fantasy football productions based on receiving yards, rushing yards, touchdowns, etc.



**Data Resource:**
[Fantasy Pros] (https://www.fantasypros.com/) Relative attributes that we are interested in from the data for our project: Position: Running Back, stats: ruhshing yards per game, rushing attempts per game(the time in which the running back carries the football), and touchdowns per game.


**Future Work:**
Following are the list of topics which if given an opportunity in future we might able to work on:
NFL running backs previous fantasy football season production
Heat map of rushing yards, receiving yards, etc. in relation to fantasy points
Pairplot to see where there is a stronger relationship for some variables such as rushing yards, touchdowns, etc. as opposed to others


Date Preprocessing

When we first started our project, we originally were going to try to predict what a NFL running back's total fantasy football point production would be. However, due to the violent nature and human aspect of the sport - we decided it would be best to predict what a running back's fantasy football point per game production will be since this will most accurately predict their true fantasy football point production while taking into account games players may miss due to injuries, illnesses, personal matters, etc.. Because we changed our dependent variable to be fantasy points per game, we also had to change the unit of measure for our original independent variables (total passing yards, total touchdowns, total rushing yards, etc.) to total passing yards per game, total touchdowns per game, total rushing yards per game, etc. so that we can accurately predict what a running back's fantasy football production will be when they are on the field. 

Data Understanding and Exploration

<img width="159" alt="Screen Shot 2021-11-13 at 3 37 01 PM" src="https://user-images.githubusercontent.com/59974878/141658337-c6159e01-72cf-4e88-9c3e-80335c1504e7.png">

<img width="158" alt="Screen Shot 2021-11-13 at 3 38 20 PM" src="https://user-images.githubusercontent.com/59974878/141658389-d6d3aac4-f554-4eab-91d7-39b41c5c8ea9.png">

Based on our pairplot above, we found that the in-game statistics such as passing yards per game, rushing yards per game, touchdowns per game, etc. were all linearly correlated with our dependent variable fantasy points per game. 

<img width="627" alt="Screen Shot 2021-11-13 at 3 39 38 PM" src="https://user-images.githubusercontent.com/59974878/141658436-7bd6417f-cabe-44b5-a4d9-70ba64eb5c62.png">

We created a heat map above to see how much of a correlation there was specifically between all of our independent variables (passing yards per game, rushing yards per game, touchdowns per game, etc.) with fantasy points per game. Based on our heat map, we found that rushing yards per game, rushing attempts per game, attempts per game, targets per game, and total touchdowns per game have the most impact on our dependent variables fantasy points per game. Rushing touchdowns per game also had a heavy impact on a NFL running backs fantasy football points per game but we decided to combine both rushing touchdowns per game and passing yards per game since total touchdowns per game will be more of an accurate indicator for how many touchdowns that particular running back will produce. 

Modeling

Evaluation

Results



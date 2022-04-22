# Data-410-Rsearch-Proposal-Draft
Draft of the proposal for final research project in DATA 410

### Introduction 
One aspect of data science that interests me a lot is its cross over between sports. One of the fields I would really like to go into as a career is using data to model and predict to help professional baseball teams optimize their results. For this reason, I have elected to do my final research using Data from Major League Baseball (MLB). In 2015 the MLB introduced _Statcast_. 

Description of Statcast"
"Statcast is a state-of-the-art tracking technology, capable of measuring previously unquantifiable aspects of the game. Set up in all 30 Major League ballparks, Statcast collects data using a series of high-resolution optical cameras along with radar equipment. The technology precisely tracks the location and movements of the ball and every player on the field, resulting in an unparalleled amount of information covering everything from the pitcher to the batter to baserunners and defensive players"

This allows for highly accurate data in all aspects of the sport. The dataset I have selected is Pitch data from 2021. I plan on using the information provided in the dataset to see how accuratly I can predict the outcome of a given pitch (hit, strike, ball, etc.).

### Data
The data set I have selected comes from Kaggle and is titled Statcast_2021. The raw data set has 93 different variables with a little over 70,000 observations. This represents every pitch thrown over the course of the season. I aim to use the model to predict the target variable "description" which is the out come of the pitch. There are 5 types of outcomes: Ball, foul, called_strike, swinging_strike, and ball_hit_into_play.

For the independent variables, some data can be eliminated immediately. There are many columns that have a majority of their values missing, so removing those columns from the data set would be beneficial. Additionally there are variables included that clearly  have no impact on the result of the ptich such as the date. There are also variables that are somewhat repetitive, for each pitcher and batter, it gives the name and the ID number so removing the names of the players would help narrow down the independent variables. 

Although there are many variables in the data set there are ones that I belive will be better predictors. This list includes: Pitch Type (Fastball, curveball etc.), pitch velocity, pitch angle, zone, release point, runners on base, spin direction, spin rate, and more. 

There are also some variables in the data set that I cannot tell what they mean. 

### Initial method ideas
I plan to apply various variable selection techniques to determine which of the 92 independent variables are statistically relevant in classifying the pitch type. Because the purpose of this research is for classification I will apply various classification techniques such as K-nearist-neighbors, decisions trees, random forest, and neural networks. 

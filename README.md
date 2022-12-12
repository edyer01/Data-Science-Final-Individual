# DataSciencePoject

## Introduction
  The objective of our project was to practice visualizing data in Python. Specifiaclly we wanted to look at data conerning videogames sales to see if we could create charts to answer the three questions we had. Those question were:
  
   1. How many games in each genre?
        
   2. Does the User_Score correlate with the Critic_Score?
    
   3. What is the breakdown of games sold on each Platform every year?


## Selection of Data
  
  The data was taken from a set found on Kaggle (https://www.kaggle.com/datasets/rush4ratio/video-game-sales-with-ratings)
  
  The data has 16 characteristics: Name, Platform, Year_of_Release, Genre, Publisher, NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales, Critic_Score, Critic_Count, User_Score, User_Count, Developer, and Rating
  
  After looking through the data, we realzied that many of our data points had incomplete infromation. We decided the best way to deal with this was to simply remove any data entry that was missing information. This took our data sample down from a size of roughly 16000 to 6000, which we felt was still enough of a smaple size to anser our questoins.

## Methods
  Tools: 
  
   All data manipualtion and visualization was done in a Juypter notebook (https://github.com/edyer01/DataSciencePoject/blob/main/DS_Final_Videogame_Data.ipynb)
   
   Pandas for data cleaning and analysis
   
   matplotlib.pyplot and seaborn for data visualization
          

## Results
  Question 1:
  ![alt text](https://github.com/edyer01/Data-Science-Final-Individual/blob/main/Q1.jpg)
  
  We decided to create a bar chart that counts the number of enteries in each genre to answer this question 
  
  Question 2:
  ![alt text](https://github.com/edyer01/Data-Science-Final-Individual/blob/main/Q2.jpg)
  
  For this question, we created a scatter plot. Along the x axis is Critic_Score and the y axis is User_Score.
  
  Question 3:
  ![alt text](https://github.com/edyer01/Data-Science-Final-Individual/blob/main/Q3.jpg)
  
  To answer this question, we decided to create a stacked area graph. Each color represents one platform, and the area of that color shows how many total games were sold globably on that specific platform for that year.

## Discussion
Question 1:

When we were trying to figure out how many games in each genre, we had to first figure out the types of genre that were already part of the dataset that we used. While combining this data we were able to figure out the final result. The highest numbers of games being in the action category, while puzzle games being the lowest amount of games produced. We used a bar graph to show the results because it helps us measure out the difference in numbers a lot easier.

Question 2:

On a quick glance, the scatter plot seems to be quite random with no obvious correlation. However, Critic and User scores are directly proportionate as there is a trend toward high scores from both parties. Despite this proportion, there are many games scattered across the plot that make pinning down a best fit line difficult. Interestingly, there are a plethora of games where User scores are higher then the Critic scores. The reason for this could be that users could be rating the game purely on how fun it is to play. The outliers, games with high scores for one party but low for the other, will be interesting to dissect to see why there is a disagreement in scores.

Question 3:
 
 The most interesting result from this graph is how quickly games sales for a platfrom drop off when a newer version of the platfrom is released. The reason behind this dropoff could be from two potential reasons. First, it could be becuase when a new version of a platform is released, video game publishers all stop publishing games on old platforms as they look to publish games on the new platform instead. Similarly, the release of a new platfrom could prompt all users of the old platfrom to stop buying games on the old platform as they have purchased the new platfrom and are purchasing games on that platfrom instead.
 
## Conclusion & Future Directions
  
  We were able to successfully able to create graphs that answered all our questions

  The the future we would like to look into the following for each questions:
  
   Q1: Use Machine Learning to try to predict which genres will have higher global sales in the future
  
   Q2: Use Scikit to create a linear regression for our User Score vs Critic Score chart to get a more precise understand of their correlation
  
   Q3: Year by year breakdowns of other categories like publisher or rating to see if any similar trends exist in those categories

 ## Individual Report (NEW WORK!!)
 
   For the individual aspect of the project, I chose to look into my groups proposed future direction to question 2:
    Use Scikit to create a linear regression for our User Score vs Critic Score chart to get a more precise understand of their correlation
    
     
   ### Results
    ![alt text](https://github.com/edyer01/Data-Science-Final-Individual/blob/main/Q4.png)
## References
  https://www.geeksforgeeks.org/pandas-groupby-multiple-values-and-plotting-results/
  https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.area.html
   https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.astype.html
   https://www.kaggle.com/datasets/rush4ratio/video-game-sales-with-ratings


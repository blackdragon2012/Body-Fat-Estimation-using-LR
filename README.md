# Body-Fat-Estimation-using-LR

![] (bfp.jpg)

source: https://fitliferegime-1eaed.kxcdn.com/wp-content/uploads/2023/05/Visual-of-Body-Fat-Percentage.webp

## Introduction:
With the rise of sedentary lifestyle and increasing unhealthy eating habits obesity has reached a new high. Many including myself somewhat lose control and failed to realise that the food we are eating is not good for us. As a data science enthusiast and now a health conscious individual, I realised that with the help of machine learning and my knowledge, I can build a model which can predict my body fat percentage.

## Motivation:

https://www.forbes.com/health/body/body-fat-percentage/ 

I came across this article which helped me understand why maintaining a health fat percentage is important and, why too little and why too much of this fat can be problematic. I won’t go into the details of the health conditions related to that.

Now the question was: How can I estimate my body fat percentage. There were some methods listed on the article, some were expensive and not readily available (DEXA scans, or Hydrostatic weighing). Then I saw a link to an online calculator which required me to fill some of my information and returns an estimated fat percentage.

https://www.forbes.com/health/body/body-fat-calculator/

This made me curious to know whether it was accurate or not. It was asking for neck, waist, hip measurements and some common questions about height, weight and age, and gave me and estimate. 
I became more curious because I believed my body stores more fat in other regions than the ones mentioned earlier. I began my hunt for a more detailed dataset, and then I found one on kaggle.

https://www.kaggle.com/datasets/fedesoriano/body-fat-prediction-dataset

This gives a more detailed measurement dataset with an estimated body fat percentage and density. All the measurements are in cms.
There are 14 independent variables and 1 dependent variable, i.e. Body Fat.

To predict an accurate percentage of body fat, I used Linear regression.

Linear regression is a statistical method used to model the relationship between a dependent variable and one or more independent variables. It assumes a linear relationship between the variables and tries to find the line of best fit that minimizes the sum of the squared errors. The resulting equation can be used to predict the value of the dependent variable for a given set of independent variables

## Results

On the last line of my notebook, we can see my estimated body fat percentage. It is ~32%, which is very high from the healthy range.

Although, the predicted result is quite close to the actual result, I made some assumptions when providing the density.

According to Katch and McArdle (1977), p. 113, a rough estimate of body fat can be calculated using this density (which can also be seen in the correlation map). And, height of an individual is very weakly correlated to the density as well as the body fat of an individual. While Abdomen was noted to be very strongly correlated to body fat, and it has been proven by many studies that most individual stores majority of fat in their abdomen area, reason being that this area has many vital organs.

## Future project ideas
- How to lose weight.
- How much money I am spending on food.


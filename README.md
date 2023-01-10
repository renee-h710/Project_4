# Team Project_4

## Team Members
Maria Hart, Taylor Shaw, Kayla Granados, Renee Holliday, Christy Martell

## Real Estate Data Summary
In the midst of another housing crisis, with prices and rates continuing to skyrocket, it is a topic on many people’s minds. Specifically, we will focus on the following areas: home value, rent percentage, and highest and lowest median housing price in 2021. We additionally predicted housing prices based on certain features and certain areas using supervised machine learning regression models. 

## Housing Values
This reflects how many houses there are per cost bracket for each state. There is a drop down menu so the user can choose which state to view the data in a bar cart format.

![image](https://user-images.githubusercontent.com/100399092/200476533-4a796849-a251-44cf-b6eb-f336f4b4dd43.png)

## Gross Rent as Percentage of Household Income
This reflects the average percentage of household income is used towards rent for California, Pennsylvania, and Puerto Rico. 

![image]()

## Highest and Lowest Median Housing Price in 2022
These maps reflect the the highest 50 and lowest 50 median housing prices in the United States.  

## Machine Learning Models
We ran extra trees regression and random forest classification models. 

Extra Trees Regression and Linear Regression are supervised machine learning models that are used to predict a continuous value output. The model takes a set of features as input and predicts a continuous value as output. The dataset used to train the models was from Kaggle.com. The “Housing Prices Dataset” contained 13 features and 545 samples. While the Extra Trees Regression model returned a higher training score, there was a large disparity between the training score and testing score. If the test score is much higher than the training score, it may indicate that the model is overfitting to the training data. For the Linear Regression Model, while the training score was not as high as the Extra Trees Regression Model, the training score and testing score were closer together, thus producing a more accurate prediction model.

Random Forest Classification: The plot gives us a visual of how unevenly our data is distributed when binned. We took the cleaned data used for the Regression Models and decided to run it through a Classification model. We first attempted to bin the data and use StandardScaler to improve accuracy. We then ran it through the Random Forest Classification model. What we observed is that the data is not equally distributed and was not easy to bin. It then returned with a training score and testing score of 1.0. This reflects the data is overfit and the model will not be able to generalize well to new, unseen data.


## Data Extracted From
- US Census Bureau - Report DP04
 - Zillow - https://www.zillow.com/research/data/     List and Sales Prices dataset

#Flask app JSON data can be found at:
https://real-estate-data.azurewebsites.net/

## Programs Used
HTML, JavaScript, Jupyter Notebook, Bootstrap, JSON, Flask app, Python, Pandas

# Team Project_4

## Team Members
Maria Hart, Taylor Shaw, Kayla Granados, Renee Holliday, Christy Martell

## Real Estate Data Summary
In the midst of another housing crisis, with prices and rates continuing to skyrocket, it is a topic on many people’s minds. Specifically, we will focus on the following areas: home value, rent percentage, and highest and lowest median housing price in 2021. We additionally predicted housing prices based on certain features and certain areas using supervised machine learning regression models. 

## Housing Values
This reflects how many houses there are per cost bracket for each state. There is a drop down menu so the user can choose which state to view the data in a bar cart format.

![image](https://user-images.githubusercontent.com/100399092/200476533-4a796849-a251-44cf-b6eb-f336f4b4dd43.png)

## Gross Rent as Percentage of Household Income

This reflects the average percentage of household income is used towards rent for California, Pennsylvania, and Puerto Rico. This was a way for us to display how much money people in each state are spending of their total income towards rent. We used Power BI and cleaned data from the Federal Census Bureau to create the pie charts. 

![image](https://user-images.githubusercontent.com/100399092/211468868-ed678065-1ccc-44c5-9a26-4357b0abe40d.png)


## Highest and Lowest Median Housing Price in 2022

These maps reflect the the highest 50 and lowest 50 median housing prices in the United States.  This would give people an idea of whether they should move to a more budget friendly area. The bubble size indicates house prices, so the bigger the bubble, the higher the house price. We chose to use red for the higher house prices to show the more expensive houses and these gradient to white as the houses decrease in price. And then on the 50 lowest home prices map we used green for the least expensive houses and these gradient to white as the home prices increase.

![image](https://user-images.githubusercontent.com/100399092/211468798-7f014445-5a37-454a-afd6-cfb4cbbcb920.png)


## Machine Learning Models

For the machine learning model, we decided to use our data in supervised machine learning regression models. These models take a set of features as input and predicts a continuous value as output. The dataset used to train the models was from Kaggle.com.  The “Housing Prices Dataset” contained 13 features and 545 samples.

ETL: As part of the model’s training and evaluation, the data was extracted from Kaggle.com and cleaned. Steps taken included downloading the csv file and reading it into a Pandas DataFrame, evaluating if there were any unnecessary columns, identifying any rows missing information, verifying datatypes and checking for outliers. The cleaned data was then loaded into a new csv file to be used for the machine learning model

We tested 8 supervised machine learning models to see which would produce the most accurate score: The eight models were the:
 * Linear Regression Model
 * Random Forest Regressor Model
 * SVR Model
 * Gradient Boosting Regressor Model
 * Extra Trees Regressor Model
 * KNeighbors Regressor Model
 * ElasticNet Model: (sklearn linear model)
 * AdaBoost Regressor Model

Observations: Some interesting observations were made. While the Extra Trees Regression model returned a higher training score (0.99), there was a large disparity between the training score and testing score (which was 0.55). If the test score is much higher than the training score, it may indicate that the model is overfitting to the training data.

For the Linear Regression Model, while the training score was not as high as the Extra Trees Regression Model, the training score and testing score were closer together, thus producing a more accurate prediction model. The training score was 0.65 and the testing score was 0.62. It is not the best scores we had hoped for, but it is not too bad.

![Extra Trees Residual Plot](https://user-images.githubusercontent.com/100399092/211468013-4da94087-fd47-4148-a513-da8718c40c2b.png)

![LR Residual Plot](https://user-images.githubusercontent.com/100399092/211468038-65d209f8-4ff9-4922-837f-32be8c0174fe.png)

Supervised Machine Learning model – Random Forest Classification 

We took the cleaned data used for the Regression Models and decided to run it through a Classification model. We first binned and scaled the data to improve accuracy. We then ran it through the Random Forest Classification model. What we observed is that the data is not equally distributed and was not easy to bin. Two features in our dataset have over a hundred unique values and the other features have only 2-4 unique values; however, those features with low unique values are important. It returned with a training score and testing score of 1.0. This reflects the data is overfit and the model will not be able to generalize well to new, unseen data.

![RandomForestClassification](https://user-images.githubusercontent.com/100399092/211468208-d35e406f-ccc5-4c00-9283-087beb3ca0f8.png)


## Data Extracted From
- US Census Bureau - Report DP04
 - Zillow - https://www.zillow.com/research/data/     List and Sales Prices dataset
 - Kaggle - https://www.kaggle.com/datasets/yasserh/housing-prices-dataset/code

#Flask app JSON data can be found at:
https://real-estate-data.azurewebsites.net/

## Tools Used
HTML, JavaScript, Jupyter Notebook, Bootstrap, JSON, Flask app, Python, Pandas,SQL, PostgreSQL, Azure, Power BI

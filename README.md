# Rossmann-Retail-Sales
Mid Course Assessment - ML Case Study

Project Name - Rossmann Retail Sales

Project Type - Regression

Contribution - Pravin Boddhul

**Project Summary -**
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

**GitHub Link -**

**Problem Statement -**
We have access to historical sales data from 1,115 Rossmann stores. Our objective is to predict the "Sales" column for the test set. It's worth noting that some stores in the dataset were temporarily closed due to renovation work.

**Data Description -**
The dataset includes two main files:

**Rossmann Stores Data.csv:** This file contains historical data, including sales information.

**store.csv:** This file provides supplemental details about the stores. Data Fields:

**Id:** An identifier representing a combination of store and date within the test set. Store: A unique identifier for each store.

**Sales:** The turnover for a particular day (this is the target variable for prediction).

**Customers:** The number of customers on a given day.

**Open:** An indicator of whether the store was open (0 = closed, 1 = open).

**StateHoliday:** Indicates a state holiday; typically, stores are closed on these days. Types include a = public holiday, b = Easter holiday, c = Christmas, 0 = None.

**SchoolHoliday:** Indicates if the store was affected by the closure of public schools on that date.

**StoreType:** Differentiates between four store models: a, b, c, d.

**Assortment:** Describes the assortment level: a = basic, b = extra, c = extended.

**CompetitionDistance:** The distance in meters to the nearest competitor store.

**CompetitionOpenSince[Month/Year]:** Approximate year and month when the nearest competitor store opened.

**Promo:** Indicates whether a store is running a promotion on that day.

**Promo2:** Indicates whether the store is participating in a continuing and consecutive promotion (0 = not participating, 1 = participating).

**Promo2Since[Year/Week]:** Describes the year and calendar week when the store started participating in Promo2.

**PromoInterval:** Describes the consecutive intervals when Promo2 is initiated, listing the months the promotion begins anew. For example, "Feb,May,Aug,Nov" indicates that the promotion restarts in February, May, August, and November of any given year for that store.

**Solution Strategy**
My strategy to solve this challenge was:

Step 01: Data Description: Use statistics metrics to identify data distributions.

Step 02: Feature Engineering: Derive new attributes based on the original variables to better describe the phenomenon that will be modeled.

Step 03: Exploratory Data Analysis: Explore the data to find insights and better understand the impact of variables on model learning.

Step 04: Feature Selection: Selection of the most significant attributes for training the model.

Step 05: Machine Learning Modelling: Machine Learning model training.

Step 06: Hyperparameter Fine Tunning: hoose the best values for each of the parameters of the model selected from the previous step.

Step 07: Convert Model Performance to Business Values: Convert the performance of the Machine Learning model into a business result.

3.Machine Learning Model Implementation and performance

At this stage models used : *Linear Regression, *Lasso Regression, *Decision Tree

![image](https://github.com/user-attachments/assets/a9be9dee-50af-4db3-8744-cb30f23a6e0b)


	  
**Conclusion**
In light of the evaluation results, it's evident that all three machine learning models, Linear Regression, Lasso Regression, and Decision Tree, exhibit varying levels of performance in predicting the target outcome.

Both Linear Regression and Lasso Regression models demonstrate similar predictive capabilities, with R-squared scores around 0.78 and Mean Squared Error values close to 0.78 as well. This suggests that they offer reasonable predictive accuracy and can effectively capture the relationships between the independent and dependent variables in the dataset.

On the other hand, the Decision Tree model stands out with remarkable performance, achieving an exceptionally high R-squared score of nearly 1 (0.999996) and a relatively low Mean Squared Error of 0.9158. These results indicate that the Decision Tree model almost perfectly predicts the target outcome and exhibits minimal prediction errors.

However, it's crucial to consider the potential drawbacks of the Decision Tree model, such as its susceptibility to overfitting, particularly in complex datasets. Despite its outstanding performance in this evaluation, further scrutiny is necessary to ascertain its generalization ability and suitability for real-world applications.

In conclusion, while all three models showcase distinct strengths and weaknesses, the Decision Tree model emerges as the top performer in terms of predictive accuracy for the given dataset. Nonetheless, careful consideration of the specific requirements and characteristics of the application domain is essential in selecting the most appropriate model for deployment.

# Capstone-Project Global Superstore

Shopping online is currently the need of the hour. Because of this COVID, it's not easy to walk in a store randomly and buy anything you want. 
We are trying to understand how is the product price varying with sales - Is there any increase in sales with the decrease in price at a day level.

Business problem statement (GOALS)
• Does product price have any impact on sales?
• IS there any way possible to improve the sales of the super stores?
• What could be the possible strategies that can be opted to cater the needs of Business.

Business Objective:
The main business objective or the challenge faced by the hypermarkets in such precedented times is how to minimize the operational expenses and
caters the need of the business stability. What should be done to face the challenges aroused due to declining sales because of the pandemic.

Approach:
Data analysis, cleaning/pre-processing: The pre-processing of the dataset before performing ML functions involves the following:

A. Structured Based Data Exploration:
It is the very first step in EDA which can also be referred to as Understanding the MetaData! That’s correct, ‘Data about the Data’. 
It is here that we get the description of the data we have in our data frame.

B. Descriptive Statistics:
Now to know about the characteristics of the data set we will use the df. describe () method which by default gives the summary of all the numerical variables present
in our data frame.

C.Handling Duplicates:
This involves 2 steps: 
1. Detecting duplicates and Removing duplicates. 
2. To check for the duplicates in our data Hereby duplicates mean the exact same observations repeating themselves. As we can see that there are no duplicate 
observations in our data and hence each observation is unique.

D.Handling Outliers:
What are Outliers? 
Outliers are the extreme values on the low and the high side of the data. 
Handling Outliers involves 2 steps: Detecting outliers and Treatment of outliers. 
Detecting Outliers For this we consider any variable from our data frame and determine the upper cut off and the lower cut-off with the help of any of the 3 methods
namely : 
• Percentile Method 
• IQR Method 
• Standard Deviation Method

Let’s consider the Purchase variable. Now we will be determining if there are any outliers in our data set using the IQR(Interquartile range) Method. 
What is this method about? You will get to know about it as we go along the process so let’s start. Finding the minimum(p0), maximum(p100), first quartile(q1), 
second quartile(q2), the third quartile(q3), and the iqr(interquartile range) of the values in the Purchase variable.

E.Outlier Treatment:
Do not worry about the data loss as here we are not going to remove any value from the variable but rather clip them. In this process, we replace the values falling
outside the range with the lower or the upper cut-off accordingly. By this, the outliers are removed from the data and we get all the data within the range.

F. Handling Missing Values:
What are Missing Values? 
Missing Values are the unknown values in the data. This involves 2 steps: Detecting the missing values and Treatment of the Missing Values.

G.Missing Value Treatment:
To treat the missing values we can opt for a method from the following : 
• Drop the variable 
• Drop the observation(s) 
• Missing Value Imputation 
For variable Product_Category_2, 31.56% of the values are missing. We should not drop such a large number of observations nor should we drop the variable itself 
hence we will go for imputation. Data Imputation is done on the Series. Here we replace the missing values with some value which could be static, mean, median, mode,
or an output of a predictive model.

H. Univariate Analysis:
In this type of analysis, we use a single variable and plot charts on it. Here the charts are created to see the distribution and the composition of the data 
depending on the type of variable namely categorical or numerical. For Continuous Variables: To see the distribution of data we create Box plots and Histograms.

Customers Analysis:
1. Profile the customers based on their frequency of purchase - calculate frequency of purchase for each customer
2. Do the high frequent customers are contributing more revenue
3. Are they also profitable - what is the profit margin across the buckets
4. Which customer segment is most profitable in each year.
5. How the customers are distributed across the countries.

Product Analysis:
1. Which country has top sales?
2. Which are the top 5 profit-making product types on a yearly basis
3. How is the product price varying with sales - Is there any increase in sales with the decrease in price at a day level
4. What is the average delivery time across the counties

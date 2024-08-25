# Customer Next Purchase Predictor

In this notebook, I will use the dataset to build an unsupervised machine learning model which allows one to estimate if a given customer will buy something again from the MH MART Limited shop in the next 14 day.

# Methodology

For this project, I followed the following steps.

# Importing relevant Python packages

   importing necessary Python libraries
   
   avoid displaying warnings
   
   import machine learning related libraries
   
# Importing Relevant Data

   In this step, I import the dataset into the Google Colab and formated the outcome variable.
   
# Data Preparation  and Data Engineering
  In this section, we will explore the given dataset to answer some general questions about the dataset. This will lead to cause us to introduce other features into the dataset which will help us to build a machine learning model that will help us to answer our main question.
  
  Also, I focused on finding and asses the missing and outliers values in the data. In other words, this step was to prepare the data for the prediction models.

# Performed an exploratory data analysis (EDA)
   In this section, i answers some questions we would like to know from the given dataset such as:
   
   * How many customers are there in the dataset and what is their Location?
   * What are the Locations that are most represented in the dataset?
   * Calculate the total NPS made in each month and what is the percentage NPS based on Branch? e.t.c.
     
# Modelling and Predicting Customer Purchase

   The goal of this section is to come up with a model using the given dataframe df_data, to estimate when a given customer is to buy or next purchasing date from MH MART LIMITED.
   
   after which i define some features and add them to the dataframe to build our machine learning model. 
   
   I use the Recency - Frequency - Monetary Value segmentation method. That is, we will put the customers into groups based on the following:

* Recency: Customers purchase behaviour based on their most recent purchase date and how many days they have been inactive since their last purchase.

* Frequency: Customers purchase behaviour based on the number of times they buy from MH MART LIMITED

* Monetary Value/Revenue: Customers purchase behaviour based the revenue they generate.

After which I apply K-means clustering to assign customers a score to each of the features.

# Machine Learning Models used in the project
1. LogisticRegression
2. GaussianNB
3. RandomForestClassifier
4. SVC
5. DecisionTreeClassifier
6. xgb.XGBClassifier(eval_metric='mlogloss')
7. KNeighborsClassifier




   

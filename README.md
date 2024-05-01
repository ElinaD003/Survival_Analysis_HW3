# Survival Analysis with Telco Customer Data

# Overview 
This repository contains Jupyter Notebook (SurvivalAnalysis.ipynb) which contains Python code for conducting survival analysis on Telco customer data. The analysis includes fitting survival models, estimating Customer Lifetime Value (CLV), and identifying at-risk subscribers for retention strategies. The aim of this project is to analyze the survival patterns of Telco customers and derive actionable insights to improve customer retention strategies. By understanding the factors influencing churn and predicting customer lifetimes, the project aims to help Telco optimize its resources and maximize customer lifetime value. 

# Data

The Telco customer data (telco.csv) contains information about customer demographics, tenure, and churn status.
Preprocessing steps include converting categorical variables into dummy variables.


# Report
The report accompanying this analysis delves into several focal points:

- Understanding Model Coefficients: This involves dissecting the significance of coefficients derived from the final survival model. It aims to unravel how various customer attributes impact churn risk and survival probabilities.
- Segmentation of Customer Base: The report focuses on segmenting customers based on their estimated Customer Lifetime Value (CLV) and churn risk. It provides insights into segments with high CLV and suggests strategies for effective retention.
- Estimation of Retention Budget: By leveraging CLV, survival probabilities, and the count of at-risk subscribers, the report estimates the annual retention budget. This aids in making data-driven decisions regarding resource allocation for retention initiatives.
- Recommendations for Retention Strategies: Customized recommendations are provided for different customer segments. These strategies aim to elevate customer satisfaction, reduce churn rates, and optimize long-term profitability.

# Parametric Models 
- Developing AFT Models: First up, we'll create our Accelerated Failure Time (AFT) models. These models come in different flavors like Weibull, Log-Normal, and Log-Logistic. They'll help us understand how various factors relate to customer survival time.
- Assessing Model Performance: Next, we'll see how well our models perform. We'll check them against different criteria to figure out which one fits our Telco customer data best. This step helps us pick the right distribution to capture survival patterns effectively.
- Visualizing Survival Trends: Time to bring our data to life! We'll plot survival curves for each model in one neat graph. This visual comparison will show us how closely each distribution matches our actual survival data.
- Choosing the Final Model: Finally, we'll decide on our go-to model. It's not just about crunching numbers – we'll also consider how easy the model is to understand, how well it fits our data, and whether it makes sense in the real world. This way, we'll land on a model that gives us valuable insights into customer survival behaviors.

# Usage
Usage

Ensure you have Python installed on your system.
Install the required libraries using pip install pandas matplotlib seaborn lifelines.
Download the SurvivalAnalysis.ipynb file and the telco.csv dataset.
Open the notebook in Jupyter or any compatible environment.
Run the code cells sequentially to perform survival analysis on the Telco customer data. 

# Analysis Steps

Fit Weibull, Log-Normal, and Log-Logistic survival models.
Plot average survival curves for each model.
Compute and print the AIC and BIC values for model comparison.
Remove irrelevant features and refit the Log-Normal survival model.
Predict survival functions, hazards, and estimate CLV.
Visualize CLV distribution based on different customer attributes.
Utilize Kaplan-Meier estimator to determine survival probabilities.
Estimate retention budget based on at-risk subscribers.


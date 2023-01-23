# JOB-A-THON-2023
Analytics Vidhya job a thon jan 2023
 
Problem Statement 

VahanBima is one of the leading insurance companies in India. It provides motor vehicle insurances at best prices with 24/7 claim settlement. It offers different types of policies for both personal and commercial vehicles. It has established its brand across different regions in India. Around 90% of the businesses today use personalized services. The company wants to launch different personalized experience programs for customers of VahanBima. The personalized experience can be dedicated resources for claim settlement, different kinds of services at doorstep, etc. Inorder to do so, they would like to segment the customers into different tiers based on their customer lifetime value (CLTV). Inorder to do it, they would like to predict the customer lifetime value based on the activity and interaction of the customer with the platform. So, as a part of this challenge, your task at hand is to build a high performance and interpretable machine learning model to predict the CLTV based on the user and policy data.

 Approach 
 
•After importing data, I did some EDA (check null values, check distributions and skewness, checked unique values etc)

•Converted object to integer using dummies python function. Dropped unwanted columns like Id(initially).

•Understand the relationship by plotting and through correlation and spearman rank corr.

•Following that I made baselines of two models Ridge and GradientBoostingRegressor. Checked which model is performing best with the help of lazy predict algorithm.

•Then, I trained all the models in 5-fold Cross-validation, experimented various techniques by trusting OOF & r2 score and taking mean of predictions on test set of all the folds

•I made observation that GradientBoostingRegressor is performing better than Ridge. 

•After that through hyper tunning found the optimized parameter for GradientBoostingRegressor Algorithm. 

•Feature Engineering – I tried transforming numerical columns by grouping various cat columns and taking mean and with standard scalar but did not gave me good score. I had tried to find the frequency and updated the train data but model didn’t gave good score.


•Through statistical model OLS (Backward elimination method procedure) removed vintage column.

•Through loss function such as Mean Absolute Error, Mean Squared Error and Root Mean Square Error analysis values for Different algorithm and parameter and finally took the best model and with parameter.

# Bank-Telemarketing-Success-Prediction-Analysis ☎️ 📊
Many times, companies face problems in effectively targeting customers, who would be willing to subscribe to long-term deposits. 
In this project I will be attempting to predict the result of a phone call to sell long-term deposits using a data modeling approach. 

# **Data**
This data contains client information relating to long term deposit subscriptions from 2008 to 2010 and it was taken from UCI Machine Learning Depository (https://archive.ics.uci.edu/dataset/222/bank+marketing). The classification goal is to predict if the client will subscribe a term deposit (variable y). The dataset includes 45,000 instances and 17 variables. 

# **Approach**
1.  Pre-processing the data using dummy encoding for categorical variables, and an 80/20  train and test split.​

2. Developed the following 6 models to apply the tests: 
- Logistic Regression
- SVM
- Decision Tree
- Random Forest
- XGBoost
- Neural Networks ​

3. Evaluated the model's performance using various metrics, such as accuracy, precision, recall, and F1-score. Recall was the metric decided to be the most important measurement of success. Here we need to select a model that gives a lower false negative rate (higher recall rate). Along with that, we validated the model on the testing dataset to ensure it generalizes well to unseen data.

4. Attempted to improve the results of models by hyperparameter tuning. I have used the lift and gain curve so see how well the model is performing as compared to a random model.

# **Results**
Based on the results that we obtained from fitting the data on various models, we found that the SVM model is giving us the highest recall score of 97 percent ( After doing hyperparameter tuning ).

In this use case, I will be focusing on a higher recall rate as we want minimum false negatives. A false negative would mean that the bank employees did not target the customers who would have bought their product. This would result in them forfeiting the full amount they could have potentially earned from the customers.

# **Recommendations**
- Based on the analysis, the SVM model can help predict potential customers which the bank marketing campaigns should target. 
- This data contains information about people living in Portugal. If we want to predict the behavior of clients living in other countries, I might have to take cultural differences and economic conditions of that country into account. But this data model can be considered as a starting point.




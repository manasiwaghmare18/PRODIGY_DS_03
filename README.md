# Prodigy_DS_03  - Build a Decision Tree Classifier 
![DS 03](https://github.com/user-attachments/assets/5d87c476-3b3d-4694-bbac-c3c63733eb4f)


# Dataset Information
Additional Information

The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. 

# There are four datasets: 
1) bank-additional-full.csv with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]
2) bank-additional.csv with 10% of the examples (4119), randomly selected from 1), and 20 inputs.
3) bank-full.csv with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs). 
4) bank.csv with 10% of the examples and 17 inputs, randomly selected from 3 (older version of this dataset with less inputs). 
The smallest datasets are provided to test more computationally demanding machine learning algorithms (e.g., SVM). 

# The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).

# Insights: 

# 1. Model Performance:

1. Both models show good performance with high accuracy on the test set. The model with the entropy criterion (dt1) has a slightly better accuracy compared to the model with the Gini criterion (dt).
   Class Imbalance:

2. Both models struggle with the minority class (class '1'), as evidenced by lower precision and recall for this class. This indicates that while the models are good at predicting the majority class (class '0'), 
   they have difficulty identifying the minority class accurately.
   Feature Importance:

3. Visualizing the decision tree helps in understanding which features are most important in making predictions. The nodes with splits based on specific features will highlight their impact on the model.

# 2. Model Improvement:

Consider tuning hyperparameters further or using techniques such as class balancing (e.g., SMOTE) to improve performance on the minority class.
Alternative models (e.g., Random Forests, Gradient Boosting) might also provide better performance and handle class imbalance more effectively.

# 3. Final Results:

1. The Decision Tree Classifier with the entropy criterion achieved the highest accuracy on the test set at 90.49%.
2. Both models show a trade-off between precision and recall, especially for the minority class, indicating potential areas for improvement.

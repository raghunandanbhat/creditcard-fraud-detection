# Credit Card Fraud Detection

Use of machine learning algorithms has the potential to significantly improve the accuracy and efficiency of credit card fraud detection. The notebooks here describe different ways of applying machine learning algorithms to identify fraudulent transactions.

### **Dataset:**
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Number of fraudulent transactions is very less compared to legitimate transactions. This imbalance is fixed using over sampling and under sampling techniques using [imbalance-learn](https://github.com/scikit-learn-contrib/imbalanced-learn)

### **Algorithms Used:**

**1. Decision Trees with Under-sampled data:**

The majority class in the dataset is clustered using KMeans clustering algorithm  to generate new set of centroids. Then the centroids are used as a new dataset representing the majority class.

**2. Decision Trees with Over-sampled data:**

New synthesized data is generated using SMOTE(Synthetic Minority Oversampling Technique) by selecting the existing  minority class samples and finding its k nearest neighbors in the feature space.

**3. Random Forest:**

Two random forests built on under-sampled and over-sampled dataset 

**4. Random Forest with XGBoost:**

Standalone random forest using [XGBoost](https://xgboost.readthedocs.io/en/stable/tutorials/rf.html)

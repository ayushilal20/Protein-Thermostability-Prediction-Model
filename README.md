# StabilityAI
Machine Learning Model for Predicting Protein Thermostability; Submitted as a part of kaggle competition for the CSE7850/CX4803 Machine Learning in Computational Biology Course.
The model utilizes k-mer count vectorization and a Gradient Boosting Regressor (GBR) to make predictions based on protein sequences.

* Data Processing:
  * Feature Engineering: K-mer count vectorization with a k-mer size of 3.
  * Tool Used: CountVectorizer from sklearn.feature_extraction.text.

* Machine Learning Model: Gradient Boosting Regressor (GBR)
  * Base Estimators: Shallow decision trees (depth of 3)
  * Number of Estimators: Initially 50, increased to 100
  * Learning Rate: Set at 0.1

* Model Training:
  * Data Split: 80% training set, 20% validation set
  * Hyperparameter Optimization: Grid search with 3-fold cross-validation
    * Final Parameters: Learning rate of 0.1, 100 estimators, max depth of 3

* Results and Conclusion:
  * The score of 0.545 on Kaggle suggests a moderate prediction accuracy.

# Diabetes-Classification
Diabetes classification project with model comparison and SMOTE-based imbalance handling.
This project focuses on building and comparing machine learning models to classify whether a person has diabetes or not. 
The goal is to identify the best-performing model while minimizing **false negatives**, which is crucial in medical diagnosis.

# Dataset
- Source: [Pima Indian Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- Selected features: `Glucose`, `BMI`, `Age`, `Insulin`

# Workflow
1. Preprocessing
   - Impute missing values (zeros replaced with median)
   - Feature selection based on importance
   - Standard scaling
2. Handling Imbalanced Data
   - Applied SMOTE oversampling on training data
3. Model Comparison
   - Compared Random Forest, K-Nearest Neighbors (KNN), and Support Vector Machine (SVM)
   - Tuned hyperparameters using GridSearchCV for Random Forest
   - Evaluated based on recall and F1-score
4. Best Result
   - Random Forest with tuned parameters gave the best balance between recall and precision
   - Achieved lower false negative rate compared to other models

# Note
This is an academic project for skill development in classification, model evaluation, and handling imbalanced data.
Due to limited time for experimentation, the SVM model was tuned with fewer hyperparameter options. 
With a more extensive search space, it is likely that the performance could be further optimized.

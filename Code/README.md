# Churn Detection Code README

## Statistical Analysis and Model Results

This README provides a detailed overview of the code and statistical analyses conducted in the churn detection project. 
The project includes the following experiments and preprocessing approaches:

### Experiment 1: StandardScaler

- **Random Forest:**
  - Mean Accuracy: 86.47%
  - Precision: 0.872, Recall: 0.856, F1 Score: 0.864
  - Confusion Matrix:
    ```
              Predicted 0  Predicted 1
    Actual 0         4475          164
    Actual 1          595          443
    ```

### Experiment 2: Cross Validation

- **Random Forest:**
  - Mean Accuracy: 86.45%
  - Precision: 0.872, Recall: 0.856, F1 Score: 0.864
  - Confusion Matrix:
    ```
              Predicted 0  Predicted 1
    Actual 0         4477          162
    Actual 1          599          439
    ```

### Experiment 3: Imputer with SMOTE

- **Random Forest:**
  - Mean Accuracy: 90.20%
  - Precision: 0.888, Recall: 0.906, F1 Score: 0.897
  - Confusion Matrix:
    ```
              Predicted 0  Predicted 1
    Actual 0         4304          385
    Actual 1          504         4056
    ```

### Original Dataset (Hot Encoding and Label Encoder)

- **Random Forest:**
  - Mean Accuracy: 86.65%
  - Precision: 0.881, Recall: 0.852, F1 Score: 0.866
  - Confusion Matrix:
    ```
              Predicted 0  Predicted 1
    Actual 0         4473          166
    Actual 1          595          443
    ```

## Model Comparison

- Random Forest consistently outperforms other models (Decision Tree, Logistic Regression, SVM, Naive Bayes, Neural Network).
- Gradient Boosting and XGBoost show competitive performance.
- Logistic Regression performs well in specific scenarios.
- Naive Bayes demonstrates the lowest performance across all datasets.

![image](https://github.com/MertBasan/churnDetection/assets/101882782/a3e20e44-598c-415b-857c-44831a7eee99)

![image](https://github.com/MertBasan/churnDetection/assets/101882782/1c973fc3-2c38-4846-b045-a8e8a4db1067)


## Preprocessing Approaches

- Resampling (SMOTE) significantly improves model performance, particularly for imbalanced datasets.
- Cross-validation provides a robust evaluation method, ensuring model reliability across different data splits.
- Standard scaling contributes to maintaining competitive model performance.
- Original data with label encoding and one-hot encoding is effective for certain models.

![image](https://github.com/MertBasan/churnDetection/assets/101882782/835e6be6-42ea-4c16-8acc-50001a843c05)

![image](https://github.com/MertBasan/churnDetection/assets/101882782/682392ab-18f2-42e7-aa0a-fd7d7a7c29cd)


Feel free to explore the code and results for a deeper understanding of the churn detection project.

**Credit Card Fraud Detection**

Detects fraudulent credit card transactions using unsupervised learning techniques on an imbalanced dataset.

This project showcases:

- How to handle class imbalances using SMOTE.
- Comparison of Logistic Regression and Random Forest.
- Evaluation with precision, recall, f1-score, and confusion matrix.


Instructions:
- Scaled Amount and Time using MinMaxScaler.
- Performed a train/test split (80/20).
- Trained Logistic Regression on imbalanced data.
- Evaluated with confusion matrix and classification report.

- Used SMOTE for balancing minority fraud cases.
- Retrained Logistic Regression on resampled data.
- Re-evaluated the model and saw a slight improvement for fraud cases.

- Trained RandomForestClassifier on SMOTE data.
- Compared performance to Logistic Regression.

Results:

Model                     | Accuracy | Precision (Fraud) | Recall (Fraud) | F1-Score (Fraud) |
Logistic Regression (SMOTE) | 0.98    | 0.06             |   0.92         |     0.11
Random Forest (SMOTE)       | 0.97    | 0.06             | 0.92           |     0.09         |

Both models had high recall but low precision, as expected in fraud detection. Also, Random Forest did perform similarly to Logistic Regression in this setup. 


Dataset:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud


# Credit Scoring Model

CodeAlpha Machine Learning Internship - Task 1

## Objective
Predict an individual's creditworthiness (good or bad credit) using past financial data.

## Dataset
German Credit dataset (credit-g, OpenML / UCI ML Repository), 1000 records.

## Approach
- Data exploration and cleaning
- Feature engineering: one-hot encoding of categorical features
- Feature scaling (StandardScaler)
- Train/test split (80/20, stratified)
- Models: Logistic Regression, Decision Tree, Random Forest
- Evaluation: Precision, Recall, F1-Score, ROC-AUC

## Results
| Model | Accuracy | ROC-AUC |
|---|---|---|
| Logistic Regression | 0.70 | 0.7529 |
| Decision Tree | 0.69 | 0.6405 |
| Random Forest | 0.72 | 0.7765 |

Best model: Random Forest (Accuracy 0.72, ROC-AUC 0.777)

Note: Recall for the bad-credit class is low (0.38 for Random Forest), so the model misses some risky applicants. Class balancing could improve this.

## Tools
Python, Pandas, Scikit-learn, Google Colab

# Overview of the Analysis

This analysis evaluates the performance of a logistic regression model in predicting credit risk. Using data from 77,536 loans, which includes borrower details like income, number of accounts, total debt, and more, the model predicts whether a loan is healthy (0) or high-risk (1). This tool can help financial institutions make informed lending decisions and reduce loan default risks.

---

## Machine Learning Process

The analysis follows these steps:

1. **Data Preparation**: Importing the dataset, organizing it into a DataFrame, and evaluating its columns.
2. **Feature and Label Separation**: Labels represent loan health (0 for healthy, 1 for high-risk), while features include all other columns.
3. **Data Splitting**: Using `train_test_split` to divide the data into training and testing sets.
4. **Model Selection**: Choosing `LogisticRegression` from the SKLearn library.
5. **Training the Model**: Fitting the logistic regression model to the training data.
6. **Making Predictions**: Using the test data to make predictions.
7. **Evaluating the Model**: Comparing metrics such as accuracy, precision, recall, and F1-scores.

---

## Results

The logistic regression model delivered strong performance:

- **Accuracy Score**: 99%
- **Precision**:
  - Healthy Loans (0): 1.00
  - High-Risk Loans (1): 0.84
- **Recall**:
  - Healthy Loans (0): 0.99
  - High-Risk Loans (1): 0.91
- **F1-Score for High-Risk Loans**: 0.91

---

## Summary

The model excels in predicting healthy loans, achieving near-perfect precision and recall. For high-risk loans, it performs well, with a recall of 0.91 (successfully identifying 91% of all high-risk loans) and a precision of 0.84 (indicating some false positives). The high accuracy and robust recall make the model a promising tool for preliminary credit risk assessments. Its ability to minimize false negatives—like overlooking high-risk loans—strengthens its utility for reducing financial risks.

However, further testing with varied datasets is recommended to ensure the model’s reliability and guard against potential overfitting, despite the large volume of data supporting its current performance.

📁 Project Title:
Loan Risk Classification using Logistic Regression

📝 Objective:
The purpose of this project is to build a logistic regression model using historical loan data to classify borrowers as either healthy (0) or high-risk (1). The model's performance is evaluated to determine if it can be reliably used by a peer-to-peer lending company to assess loan applications.

📂 Dataset:
File: lending_data.csv

Source: Provided in Resources folder

Description: This dataset includes financial attributes for loan applicants and the status of their loan: either 0 for a healthy loan or 1 for a high-risk loan.

🔧 Steps Performed:
Import Libraries: Loaded necessary libraries like Pandas, scikit-learn, and NumPy.

Load and Preview Data: Read the dataset and examined basic statistics and column structure.

Data Preparation:

Features (X) included income and debt data.

Labels (y) were derived from the loan_status column.

Data Splitting: Used train_test_split() to divide data into training and test sets (75/25), using random_state=1.

Model Training: Trained a LogisticRegression model on the training data.

Prediction: Made predictions on the testing dataset.

Evaluation: Assessed model performance using a confusion matrix and classification report.

📈 Model Evaluation:
Confusion Matrix:

lua
Copy
Edit
[[14924    77]
 [   31   476]]
Classification Report:

markdown
Copy
Edit
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     15001
           1       0.86      0.94      0.90       507

    accuracy                           0.99     15508
   macro avg       0.93      0.97      0.95     15508
weighted avg       0.99      0.99      0.99     15508
✅ Interpretation:
Accuracy: 99% – The model performs extremely well overall.

Precision (1 - High Risk): 86% – Out of all the loans predicted as high-risk, 86% were actually high-risk.

Recall (1 - High Risk): 94% – The model successfully identified 94% of actual high-risk loans.

F1-Score (1 - High Risk): 90% – A strong balance between precision and recall for identifying risky loans.

Class 0 (Healthy Loans): Extremely high precision and recall (both ~1.00), showing the model is nearly perfect in identifying safe loans.

📌 Conclusion:
The logistic regression model performs exceptionally well in classifying both healthy and high-risk loans. With an overall accuracy of 99% and strong recall for high-risk loans, this model is a reliable tool for credit risk evaluation.

Recommendation: ✅
Yes, this model is suitable for use in production with proper monitoring. It can help the company flag potentially risky borrowers and make more informed lending decisions. However, further testing with new data and possibly trying other models (e.g., Random Forest, Gradient Boosting) can be explored for comparison.

👤 Author:
Krishnaa Sigdel
📧 Email: preitysigdel@gmail.com
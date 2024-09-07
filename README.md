# Linear-Model.

For Regression:

I have created a predictive model using linear regression for loan interest rates, where I applied linear regression to predict interest rates for a peer-to-peer lending platform. Given a test and train dataset containing various details of loan applications, our task was to develop a model that accurately predicts the interest rate offered to applicants based on their inputs.

Key Highlights:

Data Analysis: I started by exploring the training data to understand the factors that influence interest rates. This involved analyzing applicant demographics, credit history, loan purpose, and more.

Feature Selection: Identified key features that impact interest rates was crucial. I focused on variables like loan amount, applicant income, credit score, and employment history.

Model Building: I used linear regression, a fundamental yet powerful statistical method, to build our predictive model. By fitting a linear equation to the observed data, I aimed to capture the relationship between the input features and the interest rates. Additionally, I implemented Ridge and Lasso regularization techniques to improve model accuracy and prevent overfitting by penalizing large coefficients.

Model Evaluation: The performance of our model was evaluated using metrics like mean squared error (MSE) and R-squared, ensuring it provides reliable predictions.

Dataset used: ld_test.csv and ld_train.csv



Classification:

Problem: A financial institution is launching a stock market trading service for its existing account holders. While the service is costly due to infrastructure, licensing, and personnel expenses, the institution plans to generate profit by charging a commission on trade transactions. However, since this service is also offered by competitors—sometimes at lower commission rates—the institution aims to attract and retain heavy traders by offering discounts. 

The challenge is that offering discounts across the board could reduce profits from customers who don't trade in large volumes. To address this, the institution wants to selectively offer discounts to customers who are likely to be heavy traders (i.e., generate significant revenue). 

To achieve this, they conducted a beta run with around 10,000 customers, manually categorizing them into two revenue categories: 
a. Revenue Category 1: Customers who are profitable (heavy traders) and should receive discounts.
b. Revenue Category 2: Customers who should not receive discounts to maintain profitability.

The goal is to use this data to build a predictive model that can identify whether a customer is likely to fall into Revenue Category 1 and, therefore, be eligible for discounts.


Approach:
- Data Collection & Preprocessing
  - Data from 10,000 customers, manually labeled into Revenue Category 1 or 2.
  - Handle missing data and encode categorical variables.
  - Scale numerical features for better model performance.

- Feature Engineering:
  - Create features such as:
    - Total trading volume.
    - Number and frequency of trades.
    - Account tenure.
    - Assets under management (AUM).
    - Previous service engagement.
    - Demographics (age, income, etc.).

- Model Selection:
  - Logistic regression chosen for binary classification (Revenue Category 1 or 2).
  - Probabilistic outputs allow threshold-based decision-making.
  - Provides interpretability through feature coefficients.

- Training the Logistic Regression Model:
  - Split data into training and test sets (e.g., 80% training, 20% test).
  - Apply regularization (L1 or L2) to prevent overfitting.

- Model Evaluation:
  - Assess accuracy on the test set.
  - Focus on precision, recall, and F1-score for business impact.
  - Analyze the confusion matrix for true positives, false positives, etc.
  - Evaluate with ROC curve and AUC score for classification performance.

- Threshold Tuning:
  - Adjust decision threshold to optimize precision (minimize incorrect discounts) and recall (maximize heavy traders captured).

- Model Interpretability:


Dataset used: bd_test.csv, bd_train.csv

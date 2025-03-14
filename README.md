# Customer Churn Analysis
Analyzed bank customers' demographics and account features using Microsoft Excel to identify factors driving customer churn, and providing insights to enhance retention efforts.

## Key Insights
![customer churn report_1.jpg](https://github.com/jakejosh6751/Customer-Retention-Analysis/blob/main/customer%20churn%20report_1.jpg)
![customer churn report_2.jpg](https://github.com/jakejosh6751/Customer-Retention-Analysis/blob/main/customer%20churn%20report_2.jpg)

- The majority of customers have not churned, but a significant portion (20%) have.
- Older customers are more likely to churn with a noticeable peak around 40s - 60s.
- Germany's churn rate is double that of France and significantly higher than Spain's, indicating an urgent need for targeted retention.
- Female customers exhibit a higher churn rate, signaling a potential need to address gender-specific preferences.
- Customers with lower credit scores have the highest churn rate.
- Inactive customers have almost double the churn rate of active customers.
- Churn risk increases sharply for high balance customers and remains moderate across mid-tier balances.
- Customers with 2 products are the most stable. Interestingly, customers with 3 or 4 products have higher churn rates.

## Common Attributes of Churners
- Age: Older
- Geography: German
- Gender: Female
- Credit Score: Lowest
- Activity Status: Inactive
- Bank Balance: Highest
- Number of Products: 3 & 4

## Key Retention Strategies
- Offer loyalty programs with perks like fee waivers and personalized services to retain highvalue customers.
- Identify and target inactive customers with tailored offers and product recommendations to reduce churn.
- Promote relevant product bundles to increase engagement and reduce churn linked to product usage. Additional data on specific products would strengthen this analysis.
- Develop targeted offers and engagement strategies for female customers.

## Churn Prediction Feasibility
Churn can be predicted using machine learning models (e.g., Logistic Regression, Random Forest) with these variables. Factors like age, bank balance, geography, and activity status would likely be strong predictors of churn.

## Techniques & Procedures

#### Data Extraction:
A dataset containing 13 features, including "Credit Score," "Geography," "Gender," and "Age," among others, with 10,000 records, was imported into Excel as a single table. Upon review, no missing data or duplicate records were identified.

#### Pivot Tables:
Pivot tables were created in separate sheets for each feature to analyze relationships with customer churn.

#### Data Cleaning Process:
Feature names and categorical values were standardized as follows:

- "CreditScore" renamed to "Credit Score."
- "NumOfProducts" renamed to "Number of Products."
- "HasCrCard" renamed to "Has Credit Card."
- "IsActiveMember" renamed to "Active Customer."
- "Exited" renamed to "Churned."
- Binary values ("0, 1") in "Has Credit Card" and "Active Customer" were converted to "No, Yes."
- Binary values ("0, 1") in "Churned" were replaced with "Retained, Churned."

#### Calculations:
The "Show Values As" % of Row Total feature in pivot tables was utilized to calculate churn percentages for categorical features and grouped numerical features.

#### Data Exploration and Visualization:
- Pie Chart: Displayed the distribution of "Retained" and "Churned" customers.
- Bar and Column Charts: Were utilized to show the percentage contribution to churn for each category for categorical features and for each aggregate for numerical features.

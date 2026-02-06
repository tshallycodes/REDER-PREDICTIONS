# Reder Telecom – Customer Churn Prediction

## Business Overview / Problem
Reder Telecom is experiencing **high customer churn** in a saturated and highly competitive telecom market. Customers switch providers due to **pricing pressure, poor network performance, lack of personalization, and weak loyalty programs**. Retention is getting harder and more expensive.

## Project Rationale
Churn prediction uses historical customer data to **identify customers likely to leave before they actually do**. This project exists for one reason: **stop revenue leakage**.

**Why it matters:**
- **Cost Reduction**: Retention is cheaper than acquisition.
- **Revenue Growth**: Longer customer lifetimes = more revenue.
- **Customer Satisfaction**: Data-driven insights improve service quality.
- **Competitive Advantage**: Act before competitors steal customers.
- **Better Decisions**: Replace guesswork with analytics.

## Project Aim
- **Build a predictive model** to identify churn-risk customers.
- **Identify key churn drivers** using feature importance and analysis.

## Data Description
The dataset is customer-level, time-stamped, and multi-source.

### Customer Profile
- Customer ID, Name, Age, Gender
- Location, Email, Phone, Address
- Segment (A / B / C)

### Purchase & Subscription
- Purchase History (Product, Frequency, Value)
- Subscription Plan, Start Date, End Date

### Digital Behavior
- Website Usage (Page Views, Time Spent)
- Clickstream Data (Action, Page, Timestamp)

### Engagement & Feedback
- Logins, Engagement Frequency (Daily / Weekly / Monthly)
- Feedback Rating (1–5), Comment
- Net Promoter Score (0–10)

### Marketing & Target
- Marketing Emails (Sent, Opened, Clicked)
- **Churn Label** (1 = churn, 0 = active)
- Record Timestamp

## Tech Stack
- **Python**
- Pandas, NumPy
- Scikit-learn

## Project Scope
- **Data Collection**: Aggregate historical customer data
- **EDA**: Understand distributions, trends, and signals
- **Preprocessing**: Encoding, scaling, cleaning
- **Feature Engineering**: Mutual information + manual pruning
- **Model Development**: Logistic Regression, Decision Tree
- **Hyperparameter Tuning**: RandomizedSearchCV
- **Evaluation**: Accuracy, Precision, Recall, F1

## Modeling Summary
- Encoded categorical features
- Trained **Logistic Regression** and **Decision Tree**
- Performed **feature selection** using mutual information
- Dropped features with MI score `< 0.01`
- Saved trained models and feature metadata

## Project Structure
├── metrics/
│ ├── dt.png
│ └── lr.png
├── model/
│ ├── logreg_model.pkl
│ ├── model.pkl # Decision Tree Model
│ ├── model.json # Feature names
│ └── model.ipynb
├── preprocessing/
│ ├──  clean_data.ipynb
│ ├──  data.csv # gitignored
│ └── cleaned_data.csv # gitignored
├── venv/
├── .env
├── requirements.txt
└── README.md

## Notes
- Raw and cleaned datasets are excluded via `.gitignore`
- This project focuses on **practical churn prediction**, not academic fluff

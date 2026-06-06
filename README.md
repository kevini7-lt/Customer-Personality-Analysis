# Customer Personality Analysis

A business data analytics and machine learning project focused on understanding customer purchasing behavior and predicting marketing campaign responses using data-driven techniques.

---

# Project Preview

## Income vs Total Spending

![Income vs Spending](figures/income_vs_spending.png)

Strong positive relationship observed between customer income and total spending.

---

## Total Spending Distribution

![Spending Distribution](figures/spending_distribution.png)

Most customers belong to the low-to-medium spending segment, while a relatively small number of customers contribute a significant portion of total revenue.

---

## Average Spending by Education

![Average Spending by Education](figures/average_spending_by_education.png)

Customers with higher education levels generally demonstrate higher average spending behavior.

---

# Business Questions

This project aims to answer the following business questions:

1. Which customer groups contribute the most revenue?
2. Does customer income influence spending behavior?
3. Does education level affect purchasing patterns?
4. Are there significant differences between customers who respond to marketing campaigns and those who do not?
5. Can machine learning be used to predict campaign responses?

---

# Dataset

Dataset: Customer Personality Analysis

Source: Kaggle: https://www.kaggle.com/datasets/imakash3011/customer
personality-analysis

Records: 2,240 customers

Features: 29 variables

The dataset contains customer demographic information, income levels, education background, purchasing history, and responses to previous marketing campaigns.

---

# Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Scikit-learn
* Jupyter Notebook

---

# Project Workflow

Raw Dataset

↓

Data Cleaning

↓

Feature Engineering

↓

Exploratory Data Analysis

↓

Statistical Analysis

↓

Customer Segmentation

↓

Machine Learning

↓

Business Insights

---

# Data Preparation

The dataset was cleaned and prepared before analysis.

Data preparation steps included:

* Handling missing values in the Income column
* Removing invalid records
* Converting customer enrollment dates into datetime format
* Creating a new feature named Total_Spending

Total_Spending was calculated by combining expenditures across multiple product categories:

* Wine
* Fruits
* Meat Products
* Fish Products
* Sweet Products
* Gold Products

---

# Exploratory Data Analysis

## Spending Distribution

The spending distribution is highly right-skewed.

Most customers are concentrated in the lower spending range, while a relatively small group of customers contributes substantially higher spending amounts.

This pattern suggests the presence of high-value customers who may be suitable targets for premium marketing strategies.

---

## Education and Spending

### Total Spending by Education Level

![Education Boxplot](figures/spending_by_education_boxplot.png)

The boxplot indicates noticeable differences in spending behavior among education groups.

Key observations:

* PhD customers exhibit the highest median spending.
* Graduation and Master groups show similar spending patterns.
* Basic education customers have significantly lower spending levels.
* Several outliers exist, indicating individual customers with exceptionally high spending behavior.

---

### Average Spending by Education

> 在这里插入图片：Average Spending by Education Bar Chart

Average spending by education level:

| Education  | Average Spending |
| ---------- | ---------------- |
| Basic      | 81.80            |
| 2n Cycle   | ~500             |
| Graduation | 621.69           |
| Master     | 609.77           |
| PhD        | 676.73           |

The results suggest a positive relationship between education level and customer spending.

---

## Income vs Spending

> 在这里插入图片：Income vs Total Spending Scatter Plot

The scatter plot reveals a strong positive relationship between income and total spending.

Key findings:

* Customers with higher income tend to spend significantly more.
* Most observations are concentrated below 100,000 annual income.
* Several extreme outliers were detected and may require further investigation.

Correlation coefficient:

0.668

This indicates a moderately strong positive relationship between income and spending behavior.

---

# Customer Segmentation

Customers were segmented into three spending categories.

| Segment         | Customers |
| --------------- | --------- |
| Low Spending    | 1231      |
| Medium Spending | 387       |
| High Spending   | 598       |

The segmentation results provide valuable information for targeted marketing campaigns and customer retention strategies.

---

# Statistical Analysis

An independent two-sample t-test was conducted to determine whether income significantly influences campaign response.

Results:

t-statistic = 6.316

p-value = 3.23 × 10⁻¹⁰

The extremely small p-value indicates a statistically significant difference in income between customers who accepted marketing offers and those who did not.

This suggests that income is an important factor affecting campaign effectiveness.

---

# Machine Learning Model

## Model

Logistic Regression

## Features Used

* Income
* Recency
* MntWines
* MntMeatProducts

## Model Performance

Accuracy = 83.1%

The model achieved strong predictive performance and demonstrates the feasibility of using machine learning techniques to identify potential campaign responders.

---

# Key Business Insights

* Income is strongly associated with customer spending behavior.
* Higher education levels are generally linked to higher spending.
* High-value customers contribute a significant share of total revenue.
* Income significantly influences marketing campaign response.
* Customer segmentation can support targeted marketing strategies.
* Predictive models can help improve marketing efficiency and campaign success rates.

---

# Repository Structure

```text
Customer-Personality-Analysis/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── customer_personality_analysis.ipynb
│
├── figures/
│   ├── spending_distribution.png
│   ├── spending_by_education_boxplot.png
│   ├── average_spending_by_education.png
│   └── income_vs_spending.png
│
└── data/
```

# Future Improvements

* Explore advanced classification models such as Random Forest and XGBoost.
* Perform feature selection and hyperparameter tuning.
* Build an interactive dashboard using Power BI or Tableau.
* Deploy the prediction model as a web application.
* Investigate the impact of outliers on model performance.

---

# Author

Li Wenjian

Computer Science Student

Skills Demonstrated:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Statistical Hypothesis Testing
* Customer Segmentation
* Machine Learning
* Business Analytics
* Data Visualization

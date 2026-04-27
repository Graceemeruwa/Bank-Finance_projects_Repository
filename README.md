## **This Repository contain some of my Fiance, Sales and Business Intellegence Projects, kindly take a look** ##


## **🏦 Bank Fraud Detection & Transaction Analysis** ##

-Unsupervised Ensemble Learning & Behavioral Risk Intelligence

## **📌 Project Overview** ##
This project implements a sophisticated Anomaly Detection Engine designed to identify fraudulent activity within high-volume banking transactions. In a financial landscape where fraud patterns evolve rapidly, this system moves beyond static rules-based alerts to an unsupervised ensemble architecture.

By integrating behavioral feature engineering with multiple mathematical outlier detection models, the system identifies "Zero-Day" anomalies—suspicious activities that have no prior known signature.

## **🛠️ Key Technical Features** ##
Behavioral Feature Engineering: Derives high-signal indicators like Transaction Velocity (time since last interaction) and Spending Deviation (ratio of transaction to user average).

Unsupervised Ensemble: Combines Isolation Forest, Local Outlier Factor (LOF), Minimum Covariance Determinant (MCD), and One-Class SVM via majority voting.

Explainable AI (XAI): Utilizes SHAP (SHapley Additive exPlanations) and Decision Tree rule extraction to provide transparent "why" behind every flag.

Business ROI Simulation: Quantifies the financial impact by balancing the Value at Risk against the Operational Cost of Review.

Fairness Audit: Evaluates model bias across customer occupations to ensure ethical and compliant flagging rates.

## **🏗️ Technical Pipeline** ##
1. Data Engineering & Optimization
Memory Management: Implemented downcasting for numeric types to optimize processing speed for large-scale datasets.

Vectorized Datetime Processing: Efficient handling of temporal features to calculate behavioral velocity.

Robust Preprocessing: Automated pipelines for LabelEncoding, StandardScaling, and handling high-cardinality categorical data.

## **2. Exploratory Data Analysis (EDA)** ##
Multivariate Distributions: Analysis of TransactionAmount, LoginAttempts, and AccountBalance.

Temporal Analysis: Identification of risk patterns across hours of the day, days of the week, and months.

Geospatial/Contextual Insights: Distribution analysis of merchant locations, channels, and device IDs.

## **3. Modeling Architecture** ##
To ensure high precision and low false-alarm rates, the system utilizes a multi-model approach:

Isolation Forest: Partitioning logic to isolate rare observations.

LOF: Density-based detection to find "hidden" anomalies in local clusters.

MCD: Mahalanobis distance estimation for robust Gaussian outlier detection.

Ensemble Voting: A robust majority-rule system that significantly reduces noise from individual model bias.

## **📈 Business Impact** ##
The project translates technical metrics into executive-level financial insights:

Value at Risk Flagged: Total monetary value of suspicious transactions identified.

Operational Efficiency: 40% reduction in manual data preparation time via vectorized workflows.

Cost-Benefit Optimization: A simulation balancing a $15.00 manual review cost against the potential loss of fraudulent transactions.

## **⚖️ Model Governance & Interpretability** ##
SHAP Summary: Provides a global view of the features driving fraud (e.g., high login attempts + abnormal spending ratios).

Interpretable Rules: Extracts human-readable "Decision Rules" (e.g., If LoginAttempts > 4 AND Amount_to_Avg_Ratio > 2.5 → Anomaly).

Fairness Review: Visualizes flagging rates across demographics to ensure alignment with banking regulatory standards and non-discrimination policies.

## **🚀 Installation & Usage** ##
Prerequisites
Python 3.10+

Jupyter Notebook or Google Colab

Setup
Clone the repository:

git clone https://github.com/your-username/bank-fraud-detection.git
Install required libraries:

pip install pandas numpy matplotlib seaborn scikit-learn shap xgboost scipy
Open and run the analysis:

jupyter notebook bank_fraud_detection_and_transaction_analysis.ipynb

## **📊 Summary of Results** ##
Anomaly Rate: Successfully identified a high-risk segment representing approximately 1.6% of total transactions.

Primary Drivers: Anomalies were primarily driven by unusual LoginAttempts, TransactionAmount deviations, and DeviceTxCount.

Visual Validation: Dimensionality reduction via t-SNE confirmed distinct clustering of anomalous transactions in low-density regions.

Developed for application in high-stakes Financial Risk Management and Data Science.


# **🚲 AdventureWorks Business Intelligence Suite** #

Global Sales, Product, and Customer Analytics Solution

## **📌 Project Overview** ##

This project transforms raw transactional data from the AdventureWorks retail database into a multi-page, interactive Business Intelligence suite. The solution provides a 360-degree view of business health, enabling stakeholders to track macro-level KPIs while drilling down into specific product performance, regional growth, and customer demographics.

## **🏗️ Data Architecture & Engineering** ##

Before visualization, a rigorous data engineering process was followed to ensure accuracy and performance:

Data Modeling: Developed a Star Schema involving 1:N relationships between Fact tables (Sales, Returns) and Dimension tables (Product, Customer, Territory, Calendar).

Power Query (ETL): Standardized currency, cleaned text strings, and optimized data types across 10+ relational tables.

DAX (Data Analysis Expressions): Created a library of custom measures including Year-to-Date (YTD) revenue, Month-over-Month (MoM) growth, and Rolling Averages for return rates.

## **📊 Dashboard Modules & Insights** ##

## **1. Executive Summary: The Macro View** ##

The primary entry point for leadership to monitor global health.

-Key Metrics: Tracking $24.9M in Revenue and $10.5M in Profit.

-Trend Analysis: A monthly revenue chart identifies seasonal peaks and growth trajectories.

-KPI Scorecards: Visual indicators for Orders vs. Targets and Return Rate stability (2.2%).

<img width="542" height="311" alt="Executive Dashboard" src="https://github.com/user-attachments/assets/ed25307e-3061-483d-a3f5-639610029b13" />

## **2. Product Intelligence: Performance & Inventory** ##

A deep dive into what is selling and what is being returned.

-Volume vs. Value: While Bikes drive the highest revenue, Accessories (like the Water Bottle - 30oz) drive the highest order frequency.

-Product Hierarchy: Analysis across Categories, Sub-categories, and individual SKUs.

-Inventory Strategy: Identifying "Top Sellers" to optimize stock levels and supply chain focus.

<img width="594" height="329" alt="products details" src="https://github.com/user-attachments/assets/27cc430f-13ca-4f46-b49e-25d0cc76a33a" />


## **3. Customer Analytics: Demographic Profiling** ##

Understanding the "who" behind the revenue.

-Occupational Trends: Analysis shows that Professionals and those in Management contribute the highest revenue share.

-Top Individual Customers: Identifying "Whale" customers (e.g., Maurice Shan and Janet Munoz) for potential loyalty or targeted marketing campaigns.

-Revenue Per Customer: Tracking the average value of the customer base over time.

<img width="594" height="329" alt="Customers details" src="https://github.com/user-attachments/assets/358843cd-5d74-4c51-88f8-f0c0bcb3fcdf" />

## **4. Geospatial Performance: Regional Deep-Dive** ##

Interactive mapping of the global footprint.

-Market Dominance: North America remains the primary revenue engine, followed by Europe and Australia.

-Order Distribution: Visualizing order density across specific territories to identify untapped market opportunities.

-Regional Filtering: Stakeholders can filter the entire report suite by clicking on specific continents or regions.

<img width="593" height="337" alt="Geographical insights" src="https://github.com/user-attachments/assets/c7a1b68e-6bfe-4575-b87f-3a21635d97f5" />

## **💡 Key Actionable Insights** ##

-Retention Opportunity: Professionals represent the highest-spending segment; marketing efforts should focus on high-end bike models for this demographic.

-Product Optimization: Accessories have high volume but low margin; bundling these with high-margin Bike purchases could increase the Average Order Value (AOV).

-Geographic Expansion: The Pacific/Australian market shows high order density relative to its size, suggesting a strong candidate for regional warehouse expansion to reduce shipping costs.

**🛠️ Tools Used**

-Power BI Desktop: Report Authoring & DAX.

-Power Query: Data Cleaning & ETL.

-DAX: Time-Intelligence & Advanced Calculations.

-Star Schema: Relational Data Modeling.

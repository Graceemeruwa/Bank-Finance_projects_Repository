***🏦 Bank Fraud Detection & Transaction Analysis***

-Unsupervised Ensemble Learning & Behavioral Risk Intelligence
**📌 Project Overview**
This project implements a sophisticated Anomaly Detection Engine designed to identify fraudulent activity within high-volume banking transactions. In a financial landscape where fraud patterns evolve rapidly, this system moves beyond static rules-based alerts to an unsupervised ensemble architecture.

By integrating behavioral feature engineering with multiple mathematical outlier detection models, the system identifies "Zero-Day" anomalies—suspicious activities that have no prior known signature.

**🛠️ Key Technical Features**
Behavioral Feature Engineering: Derives high-signal indicators like Transaction Velocity (time since last interaction) and Spending Deviation (ratio of transaction to user average).

Unsupervised Ensemble: Combines Isolation Forest, Local Outlier Factor (LOF), Minimum Covariance Determinant (MCD), and One-Class SVM via majority voting.

Explainable AI (XAI): Utilizes SHAP (SHapley Additive exPlanations) and Decision Tree rule extraction to provide transparent "why" behind every flag.

Business ROI Simulation: Quantifies the financial impact by balancing the Value at Risk against the Operational Cost of Review.

Fairness Audit: Evaluates model bias across customer occupations to ensure ethical and compliant flagging rates.

**🏗️ Technical Pipeline**
1. Data Engineering & Optimization
Memory Management: Implemented downcasting for numeric types to optimize processing speed for large-scale datasets.

Vectorized Datetime Processing: Efficient handling of temporal features to calculate behavioral velocity.

Robust Preprocessing: Automated pipelines for LabelEncoding, StandardScaling, and handling high-cardinality categorical data.

**2. Exploratory Data Analysis (EDA)**
Multivariate Distributions: Analysis of TransactionAmount, LoginAttempts, and AccountBalance.

Temporal Analysis: Identification of risk patterns across hours of the day, days of the week, and months.

Geospatial/Contextual Insights: Distribution analysis of merchant locations, channels, and device IDs.

**3. Modeling Architecture**
To ensure high precision and low false-alarm rates, the system utilizes a multi-model approach:

Isolation Forest: Partitioning logic to isolate rare observations.

LOF: Density-based detection to find "hidden" anomalies in local clusters.

MCD: Mahalanobis distance estimation for robust Gaussian outlier detection.

Ensemble Voting: A robust majority-rule system that significantly reduces noise from individual model bias.

**📈 Business Impact**
The project translates technical metrics into executive-level financial insights:

Value at Risk Flagged: Total monetary value of suspicious transactions identified.

Operational Efficiency: 40% reduction in manual data preparation time via vectorized workflows.

Cost-Benefit Optimization: A simulation balancing a $15.00 manual review cost against the potential loss of fraudulent transactions.

**⚖️ Model Governance & Interpretability**
SHAP Summary: Provides a global view of the features driving fraud (e.g., high login attempts + abnormal spending ratios).

Interpretable Rules: Extracts human-readable "Decision Rules" (e.g., If LoginAttempts > 4 AND Amount_to_Avg_Ratio > 2.5 → Anomaly).

Fairness Review: Visualizes flagging rates across demographics to ensure alignment with banking regulatory standards and non-discrimination policies.

**🚀 Installation & Usage**
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
📊 Summary of Results
Anomaly Rate: Successfully identified a high-risk segment representing approximately 1.6% of total transactions.

Primary Drivers: Anomalies were primarily driven by unusual LoginAttempts, TransactionAmount deviations, and DeviceTxCount.

Visual Validation: Dimensionality reduction via t-SNE confirmed distinct clustering of anomalous transactions in low-density regions.

Developed for application in high-stakes Financial Risk Management and Data Science.

Retail Customer Segmentation & Sales Analysis

This project focuses on analyzing e-commerce customer transaction data using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering to identify distinct customer segments. The analysis is further supported by an interactive Streamlit dashboard to visualize segment-wise insights and behaviors, assisting businesses in data-driven decision-making for customer targeting and retention strategies.

Objective

To develop a customer segmentation model that classifies customers based on purchasing behavior, helping marketing and sales teams target different customer groups more effectively.

Project Summary

- Performed exploratory data analysis (EDA) on real-world e-commerce data to uncover trends and irregularities.
- Cleaned and preprocessed data, addressing null values, duplicates, cancellations, and outliers.
- Calculated RFM metrics to quantify customer behavior over time.
- Applied K-Means clustering to group customers into actionable segments.
- VisualizedRetail-Customer-Segmentation/
│
├── data/ # Raw & processed data files
│ └── online_retail.csv
│
├── notebooks/ # Jupyter notebooks (4 stages of analysis)
│ ├── 01_EDA_and_Cleaning.ipynb
│ ├── 02_RFM_Analysis.ipynb
│ ├── 03_Clustering_KMeans.ipynb
│ └── 04_Insights_Visualization.ipynb
│
├── dashboard/ # Streamlit app
│ ├── app.py
│ └── rfm_clustered.csv
│
├── reports/ # Final summary report (PDF)
│ └── final_report.pdf
│
├── requirements.txt # List of required Python packages
└── README.md # Project overview


Methodology

1. Data Exploration & Cleaning
- Dataset: [UCI Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail)
- Removed missing customer IDs, negative quantities (returns), and cancelled invoices.
- Converted date fields and created additional date-based features.

2. RFM Analysis
- Recency: Days since the last purchase.
- Frequency: Total number of purchases.
- Monetary: Total amount spent.
- Each customer was scored and ranked using quantile-based segmentation.

3. Customer Segmentation with K-Means
- Used Elbow Method and Silhouette Score to determine optimal number of clusters.
- Applied K-Means to standardized RFM data.
- Clustered customers into 4 segments based on behavioral patterns.

 4. Insights & Business Interpretation
- Plotted boxplots and bar charts to compare clusters.
- Identified high-value, at-risk, and potential churn customers.
- Suggested actionable marketing strategies for each group.

 5. Streamlit Dashboard
- Built an interactive dashboard to display:
  - Cluster distribution
  - Customer-level RFM scores
  - Visual breakdowns for each segment
- Enables business users to explore data without writing code.

 Key Insights

- Cluster 0: High-value frequent buyers — suitable for loyalty rewards.
- Cluster 1: Recent but low-frequency buyers — ideal for cross-sell promotions.
- Cluster 2: Inactive customers — need reactivation campaigns.
- Cluster 3: Low engagement & low spend — may be deprioritized in campaigns.

Tools & Technologies

- Languages : Python  
- Libraries : Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Streamlit  
- Environment : Jupyter Notebook, Google Colab  
- Version Control : Git & GitHub

 

Final Deliverables

- Cleaned dataset (`rfm_clustered.csv`)
- Four well-documented Jupyter notebooks
- Streamlit dashboard for business insights
- PDF report summarizing the entire pipeline and conclusions
- GitHub repository with structured folders and README

Author

Vanshika Tonk
B.Tech Computer Science (AIML) | Aspiring Data Analyst  
🔗 [LinkedIn](https://linkedin.com/in/yourprofile) | 📧 [vanshikatonk012@gmail.com]

 Note

This project is intended to showcase skills in data analysis, segmentation modeling, dashboard creation, and business communication. It can be extended by integrating predictive modeling, web scraping, or real-time customer data APIs in future versions.



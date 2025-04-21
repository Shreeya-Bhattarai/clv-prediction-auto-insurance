# Customer Lifetime Value Optimization through Segmentation and Predictive Modeling
This repository contains the code, models, and methodology used in my MSc Data Analytics thesis at Lund University. This project analyzes customer lifetime value (CLV) from a U.S. auto insurance company to identify key value drivers and segment customers into distinct clusters. Using clustering and machine learning models, we propose data-driven retention and upsell strategies for each customer segment, increasing marketing ROI and customer satisfaction.

### Objective of the study
Auto insurance companies often struggle to identify which customers are most valuable over time. A one-size-fits-all marketing strategy leads to missed opportunities and wasted spend. This analysis aims to:
    - Identify the key drivers of Customer Lifetime Value (CLV)
    - Segment customers based on business value
    - Recommend tailored retention and upsell strategies
    
### Dataset
The dataset is obtained directly from Kaggle and belongs to an auto insurance company in the USA. The data is recorded for a period of two months between 1st January 2011 and 28th
February 2011. It contains information about every policyholder’s vehicle, policy type, and socio-economic status. There are 24 columns and 9134 unique values in the dataset. The data has no missing values.

### Data Analysis Approach
- EDA: Identified strong correlations between CLV and features like Monthly Premium, Number of Policies, Total Claim Amount, and Income.
- Segmentation: Applied PCA for dimensionality reduction and k-means clustering. Identified 3 distinct customer segments by CLV.
- Modeling: Trained Random Forest, XGBoost, and Neural Networks to predict CLV. Best results came from training per-cluster models (up to R² = 0.955).
- Business Recommendations: Used each cluster characteristics to recommend marketing and retention strategies.

### Model Performance

| Model         | R² (Clustered) |
|---------------|----------------|
| Random Forest | 0.955          |
| XGBoost       | 0.801          |
| Neural Net    | 0.822          |

All models showed improved performance when trained on clustered data due to more homogenous group characteristics, with Random Forest achieving the highest overall R².

### Insights
- Customers in California and Oregon make up 60% of revenue → targeted geo-retention.
- High CLV = higher premiums + more policies → upsell opportunities.
- Segment 3 (high CLV): propose loyalty club, fast-track renewals, and dedicated service line.
- Segment 1 & 2: use assigned agents and policy communication to increase engagement.

### Technologies Used
- Python (Pandas, Scikit-learn, XGBoost, Seaborn)
- Jupyter Notebooks
- KMeans, PCA
- Random Forest, XGBoost, Neural Network
  



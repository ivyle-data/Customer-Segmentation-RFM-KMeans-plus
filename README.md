# RFM Customer Segmentation with K-Means++
This project performs customer segmentation using RFM (Recency, Frequency, Monetary) analysis and K-Means++ clustering.

## Project Overview
Understanding customer behavior is essential for effective marketing and business decision-making. This project applies RFM analysis and K-Means++ clustering to segment customers based on their purchasing patterns.
## Dataset
- Source: Adventure Works Cycles (virtual dataset).
- Contains **121,253 transactions** from **01/07/2017 to 15/07/2020**.
- Filtered to **United States market**.
## Technologies Used
- **Google Colab** (Jupyter-based environment)
- **Python Libraries**:
  - **Data Processing & Feature Engineering:**
    - `pandas`, `numpy`, `scipy.stats`
  - **Data Visualization:**
    - `matplotlib`, `seaborn`, `squarify`
  - **Machine Learning & Clustering:**
    - `sklearn.cluster` → **KMeans (clustering)**
    - `sklearn.preprocessing` → **StandardScaler (feature scaling)**
    - `sklearn.metrics` → **Silhouette Score, Davies-Bouldin Score, Calinski-Harabasz Score (clustering evaluation)**
  
## Key Steps
1. **Data Cleaning & Preprocessing**
   - Handle missing values
   - Convert dates and transaction formats
2. **Feature Engineering**
   - Compute Recency, Frequency, and Monetary (RFM) values
   - Normalize data for clustering
3. **Customer Segmentation**
   - Use **K-Means++** clustering to group customers
   - Analyze cluster characteristics
4. **Visualization & Insights**
   - Generate scatter plots for customer segmentation.

## Results
- Identified **7 customer segments** by RFM analysis (Unsteady Customers, Lost Customers, Potential Lost Customers, At-Risk Customers, Emerging Customers, Active Customers, Inactive Customers, Top Customers).
- Identified **3 customer clusters** (Gold, Silver, Bronze) by K-Means++ clustering model based on RFM values.
- Provided actionable insights to improve marketing strategies.

## How to Run the Project
Click this Google Colab Notebook
[![Open in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1OKcdIpSASCmx8LGRgdIkYl9l6oUbe4BR?usp=sharing)
Or:
1. Open Google Colab: [Colab Notebook](https://colab.research.google.com/)
2. Upload the notebook (`rfm_analysis.ipynb`)
3. Install dependencies (if needed) by running:
   ```python
   !pip install squarify scikit-learn-extra lifetimes

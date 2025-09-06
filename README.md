# Customer Segmentation Analysis (Clustering Models)

## Overview
This project performs **Customer Segmentation** using multiple clustering techniques.  
The aim is to group mall customers based on **Age, Annual Income, and Spending Score**, and to transform these technical results into **business insights** that can guide marketing and customer relationship management.

---

## Dataset
- **Source:** Mall Customers dataset (200 customers)  
- **Attributes:**  
  - CustomerID  
  - Gender  
  - Age  
  - Annual Income (k$)  
  - Spending Score (1-100)  

---

## Methodology

### 1. Data Exploration & Preprocessing
- Checked dataset shape, datatypes, and summary statistics.  
- Plotted distributions of Age, Annual Income, Spending Score.  
- Used pairplots to observe relationships and gender differences.  

### 2. Clustering Methods
- **k-Means**: Optimal clusters found via **Elbow Method** → k = 5  
- **Hierarchical Clustering**: Used Ward linkage to form dendrograms  
- **DBSCAN**: Density-based clustering for irregular shapes  
- **BIRCH**: Efficient clustering for large datasets  

### 3. Model Comparison
To test clustering quality, hybrid approaches with ML models were tried:  
- Random Forest, Gradient Boosting, AdaBoost combined with cluster outputs.  
- Metrics: MSE (Mean Squared Error), Explained Variance, Processing Time.  

---

## Key Findings

### Segments from k-Means (k=5):
1. **Young – High Spend**  
   - Younger customers with strong buying habits.  
   - Business insight: focus loyalty programs & trend campaigns.  

2. **High Income – Low Spend**  
   - Affluent but not actively spending.  
   - Insight: Use CRM data to identify this group and target with tailored offers such as premium campaigns and exclusive offers (personalized discounts, loyalty       privileges) to unlock their revenue potential.

3. **Average Profile**  
   - Medium income, medium spending.  
   - Insight: stable customer base, protect with retention plans.  

4. **Low Income – Low Spend**  
   - Price-sensitive group.  
   - Insight: target with bundles, discounts, affordable products.  

5. **Mature – Balanced Spending**  
   - Older customers with consistent habits.  
   - Insight: cross-sell services, maintain loyalty.  

### Other Clustering Models:
- **Hierarchical & BIRCH** produced similar groups, validating k-means findings.  
- **DBSCAN** marked some customers as outliers, useful for anomaly detection.  

### Model Performance:
- Gradient Boosting & AdaBoost showed better explained variance than Random Forest.  
- AdaBoost + DBSCAN combination highlighted distinct spending patterns.  

---

## Business Value
- Enables **targeted marketing campaigns** per segment.  
- Identifies **untapped high-income customers**.  
- Protects revenue through **churn prevention** strategies.  
- Helps managers **allocate resources** effectively.  

---

## Visuals
Key plots included in analysis:
- Distribution histograms of Age, Income, Spending Score  
- Pairplots with gender breakdown  
- Elbow Method for optimal k  
- 2D & 3D cluster scatter plots  
- Comparison of clustering methods (k-Means, DBSCAN, BIRCH)  

---

## Technologies
- **Python**: pandas, numpy, matplotlib, seaborn, scikit-learn  
- **Clustering Models**: k-Means, DBSCAN, Hierarchical, BIRCH  
- **Machine Learning**: Random Forest, Gradient Boosting, AdaBoost  

---



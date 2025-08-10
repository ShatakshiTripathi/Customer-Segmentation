# Customer Segmentation with K-Means and PCA

## Project Overview

This project performs customer segmentation using the **Mall Customers Dataset** by applying **K-Means clustering** enhanced with **Principal Component Analysis (PCA)** for dimensionality reduction.

The goal is to identify distinct customer groups based on demographics and spending behavior to enable targeted marketing strategies.

---

## Dataset

The dataset used is the [Mall Customers Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) downloaded from Kaggle.

**Features include:**

- CustomerID: Unique identifier
- Gender: Male or Female
- Age: Customer age
- Annual Income (k$): Annual income in thousand dollars
- Spending Score (1-100): Score assigned by the mall based on customer behavior and spending

---

## Project Steps

1. **Exploratory Data Analysis (EDA):**  
   - Understand dataset structure, check missing values  
   - Visualize distributions of Age, Gender, Income, and Spending Score  
   - Identify relationships between features  

2. **Data Preprocessing:**  
   - Encode categorical variables (Gender) numerically  
   - Scale features using StandardScaler to standardize data  

3. **Dimensionality Reduction (PCA):**  
   - Reduce dataset dimensionality to 2 principal components for visualization  
   - Analyze explained variance by PCA components  

4. **Determining Optimal Number of Clusters:**  
   - Use Elbow method (inertia) and Silhouette scores to find best `k` for K-Means  

5. **K-Means Clustering:**  
   - Apply K-Means with optimal cluster count  
   - Visualize clusters in PCA-transformed 2D space  

6. **Cluster Profiling:**  
   - Analyze mean and spread of features within each cluster  
   - Use visualizations (boxplots, count plots) to understand cluster characteristics  

7. **Business Insights & Targeting Strategies:**  
   - Propose actionable marketing strategies based on cluster profiles  
   - For example, premium offers for high income & spending score clusters, discounts for low engagement clusters  

8. **Saving Results:**  
   - Export segmented data with cluster labels  
   - Save trained K-Means model for future use (optional)  

---

## How to Run

1. Download `Mall_Customers.csv` from [Kaggle dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).
2. Place the CSV in your working directory or upload it to your Colab environment.
3. Install required Python libraries if not installed:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn joblib

# 🛍️ Mall Shopper Segmentation using Unsupervised Learning

## 📌 Project Overview

This project performs **Customer Segmentation** using **Unsupervised Machine Learning** techniques on the Mall Customer Segmentation dataset. Three clustering algorithms—**K-Means**, **Agglomerative Hierarchical Clustering**, and **DBSCAN**—were implemented and compared to identify meaningful customer groups.

The project includes data preprocessing, feature engineering, clustering analysis, customer profiling, algorithm comparison, business recommendations, and deployment using a machine learning pipeline.

---

📺 **Presentation Video:**  
👉 **https://drive.google.com/file/d/1m1Pz9JP2Sfpnx1umIARnN8UKMJ_rWODc/view?usp=sharing**

---

# 🎯 Objectives

- Analyze customer demographic and spending behavior.
- Perform customer segmentation using clustering algorithms.
- Compare multiple clustering techniques.
- Evaluate clustering quality using internal validation metrics.
- Identify meaningful customer personas.
- Provide business recommendations based on customer segments.
- Build a deployment-ready clustering pipeline.

---

# 📂 Dataset

- **Dataset:** Mall Customer Segmentation
- **Learning Type:** Unsupervised Learning
- **Number of Records:** 200 Customers

### Features

- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

The dataset does not contain a target variable because clustering is an unsupervised learning problem.

---

# 🚀 Project Workflow

## 📖 Step 1 – Dataset Loading & Exploratory Data Analysis (EDA)

Performed:

- Loaded the dataset
- Checked missing values
- Checked duplicate values
- Statistical summary
- Gender distribution
- Age distribution
- Annual Income distribution
- Spending Score distribution
- Correlation analysis
- Data visualization

<p align="center">
<img src="FINAL-Pratical/IMAGES/eda.jpeg.png" width="850">
</p>

---

## ⚙️ Step 2 – Feature Engineering & Data Preprocessing

Performed:

- Renamed column names
- Label Encoding
- Income Group creation
- Age Group creation
- Spending Category creation
- Standard Scaling
- Feature Selection

<p align="center">
<img src="FINAL-Pratical/IMAGES/preprocessing.jpeg.png" width="850">
</p>

---

## 🤖 Step 3 – K-Means Clustering

Implemented:

- Elbow Method
- Silhouette Analysis
- Optimal Cluster Selection
- Final K-Means Model
- PCA Visualization
- Cluster Profiling
- Customer Personas

<p align="center">
<img src="FINAL-Pratical/IMAGES/kmeans.jpeg.png" width="850">
</p>

---

## 🌲 Step 4 – Agglomerative Hierarchical Clustering

Implemented:

- Ward Linkage
- Complete Linkage
- Average Linkage
- Dendrogram Analysis
- Cluster Visualization
- Cluster Profiling

<p align="center">
<img src="FINAL-Pratical/IMAGES/agglomerative.jpeg.png" width="850">
</p>

---

## 🚀 Step 5 – DBSCAN Clustering

Implemented:

- k-Nearest Neighbor Distance Plot
- Epsilon Selection
- DBSCAN Model
- Noise Detection
- Cluster Visualization
- Customer Profiling

<p align="center">
<img src="FINAL-Pratical/IMAGES/dbscan.jpeg.png" width="850">
</p>

---

## 📈 Step 6 – Model Evaluation & Comparison

Compared the following clustering algorithms:

- K-Means
- Agglomerative Clustering
- DBSCAN

Evaluation Metrics:

- Silhouette Score
- Davies–Bouldin Index
- Calinski–Harabasz Index

Additional Analysis:

- K-Means Stability Check
- Business Recommendation

<p align="center">
<img src="FINAL-Pratical/IMAGES/comparison.jpeg.png" width="850">
</p>

---

## 💼 Step 7 – Deployment & Business Recommendation

Deployment includes:

- Saving StandardScaler
- Saving K-Means Model
- Shopper Classification Function
- Prediction for New Customers
- Customer Persona Recommendation

Business Recommendation includes:

- Personalized Marketing
- Customer Retention Strategy
- Loyalty Programs
- Premium Membership Plans
- Store Layout Optimization

<p align="center">
<img src="FINAL-Pratical/IMAGES/business.jpeg.png" width="850">
</p>

---

# 🏆 Best Performing Algorithm

**K-Means Clustering** achieved the best overall performance.

### Why?

- Highest Silhouette Score
- Lowest Davies–Bouldin Index
- High Calinski–Harabasz Score
- Stable across multiple random states
- Computationally efficient
- Easy to interpret
- Suitable for large customer datasets

---

# 👥 Customer Personas

The project identified five major customer groups:

### 💎 Big Spenders

- High Income
- High Spending

Recommendation:

- VIP Membership
- Luxury Brand Promotions
- Exclusive Events

---

### 🛒 Budget Shoppers

- Low Income
- Low Spending

Recommendation:

- Discount Coupons
- Cashback Offers
- Seasonal Sales

---

### 🎯 Careful Spenders

- Moderate Income
- Balanced Spending

Recommendation:

- Loyalty Rewards
- Personalized Coupons
- Bundle Offers

---

### 🌟 Young Aspirers

- Young Customers
- High Spending Interest

Recommendation:

- Fashion Campaigns
- Student Discounts
- Entertainment Packages

---

### 👨‍👩‍👧 Mature Savers

- High Income
- Conservative Spending

Recommendation:

- Family Shopping Plans
- Wellness Programs
- Premium Services

---

# 📦 Deployment

The final clustering model was saved using **Joblib**.

```python
import joblib

model = joblib.load("mall_segmentation_model.pkl")
scaler = joblib.load("mall_scaler.pkl")
```

Prediction for a new shopper:

```python
cluster = model.predict(scaler.transform([[AnnualIncome, SpendingScore]]))
```

---

# 📁 Repository Structure

```text
mall-shopper-segmentation-unsupervised-learning/
│
├── MallShopperSegmentation.ipynb
├── mall_segmentation_model.pkl
├── mall_scaler.pkl
├── README.md
├── requirements.txt
├── summary_report.md
│
└── IMAGES/
    ├── eda.jpeg
    ├── preprocessing.jpeg
    ├── kmeans.jpeg
    ├── agglomerative.jpeg
    ├── dbscan.jpeg
    ├── comparison.jpeg
    └── business.jpeg
```

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- Joblib
- Jupyter Notebook

---

# ▶️ Installation

Clone the repository:

```bash
git clone https://github.com/sanikale03/mall-shopper-segmentation-unsupervised-learning
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook:

```bash
jupyter notebook
```

Open:

```text
MallShopperSegmentation.ipynb
```

Run all cells in sequence.

---

# 📌 Key Learnings

- Unsupervised Learning
- Customer Segmentation
- Feature Engineering
- Data Visualization
- K-Means Clustering
- Agglomerative Clustering
- DBSCAN
- Cluster Evaluation Metrics
- Customer Profiling
- Business Recommendation
- Model Deployment using Joblib

---

# 🚀 Future Scope

- Include transaction history
- Purchase category analysis
- Loyalty card information
- Visit frequency analysis
- Real-time customer segmentation
- Power BI Dashboard
- Recommendation System Integration

---

# 👩‍💻 Author

**Sanika Kale**

MCA Student | Data Analytics , AI  & Machine Learning

Red & White Skill Education

---

⭐ **If you found this project useful, consider giving it a star on GitHub!**
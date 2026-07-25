# 📄 Summary Report

# Mall Shopper Segmentation using Unsupervised Learning

---

## 📌 Business Problem

Shopping malls serve customers with different income levels, age groups, and purchasing behaviors. Treating all customers the same often leads to ineffective marketing campaigns, lower customer engagement, and reduced sales.

The objective of this project is to identify meaningful customer groups using **Unsupervised Machine Learning** so that the retail management team can design personalized marketing strategies, improve customer satisfaction, and increase overall business revenue.

Since there are no predefined target labels in the dataset, clustering algorithms are used to discover hidden customer segments based on shopping patterns.

---

# 📂 Dataset Description

The **Mall Customer Segmentation** dataset contains demographic and spending information of mall customers.

### Features Used

- Customer ID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

The project primarily used **Annual Income** and **Spending Score** for 2D clustering, while additional features such as **Age** and **Gender** were included for higher-dimensional analysis.

---

# ⚙️ Data Preprocessing & Feature Engineering

The following preprocessing steps were performed before applying clustering algorithms:

- Checked missing values
- Removed duplicate records
- Renamed column names
- Label encoded the Gender column
- Created Income Groups
- Created Age Groups
- Created Spending Categories
- Standardized numerical features using StandardScaler

Feature scaling ensured that all variables contributed equally to the clustering process.

---

# 🤖 Clustering Algorithms Implemented

Three clustering algorithms were implemented and compared.

## 1. K-Means Clustering

K-Means clustering was used to partition customers into distinct groups. The optimal number of clusters was selected using the **Elbow Method** and validated using the **Silhouette Score**. Customer personas were created by analyzing the characteristics of each cluster.

---

## 2. Agglomerative Hierarchical Clustering

Agglomerative Clustering grouped customers based on hierarchical relationships. Different linkage methods such as **Ward**, **Complete**, and **Average Linkage** were evaluated using dendrograms and silhouette analysis.

---

## 3. DBSCAN

DBSCAN was applied to identify dense customer groups and detect noise or outlier customers. The epsilon value was selected using the **k-Nearest Neighbor Distance Plot**, allowing the model to identify customers who did not belong to any major cluster.

---

# 📊 Model Evaluation

The clustering algorithms were evaluated using internal validation metrics:

- Silhouette Score
- Davies–Bouldin Index
- Calinski–Harabasz Index

Additionally, K-Means stability was verified by training the model using multiple random states. The results demonstrated consistent clustering performance across different initializations, confirming that the algorithm is reliable for this dataset.

---

# 🏆 Best Performing Algorithm

Among all three clustering techniques, **K-Means Clustering** was selected as the best-performing algorithm because:

- Produced well-separated customer clusters.
- Achieved the best overall clustering quality according to evaluation metrics.
- Showed stable results across multiple executions.
- Computationally efficient and scalable.
- Easy to interpret for business users.

Agglomerative Clustering produced similar customer segments but required higher computational effort, while DBSCAN was effective for detecting outlier customers.

---

# 👥 Customer Segments

The analysis identified five major customer groups:

### 💰 Big Spenders

Customers with high income and high spending behavior.

**Business Strategy**

- Premium membership
- Luxury product promotions
- Exclusive shopping events

---

### 🛒 Budget Shoppers

Customers with low income and low spending.

**Business Strategy**

- Discounts
- Cashback offers
- Seasonal promotions

---

### 🎯 Careful Spenders

Customers with moderate income and planned spending behavior.

**Business Strategy**

- Loyalty rewards
- Personalized coupons
- Bundle offers

---

### 🌟 Young Aspirers

Young customers with relatively lower income but high spending interest.

**Business Strategy**

- Fashion campaigns
- Student discounts
- Entertainment offers

---

### 👨‍👩‍👧 Mature Savers

Customers with high income but conservative spending habits.

**Business Strategy**

- Family shopping packages
- Wellness and lifestyle promotions
- Premium service memberships

---

# 💼 Business Recommendation

Based on the clustering results, **K-Means Clustering** is recommended for deployment in the mall's customer analytics system.

The identified customer segments can be used to:

- Personalize marketing campaigns.
- Improve customer engagement.
- Increase customer retention.
- Optimize store placement.
- Design targeted loyalty programs.
- Improve overall shopping experience.

Using customer segmentation enables retailers to make informed business decisions and maximize revenue through targeted promotions.

---

# 🚀 Future Improvements

The current dataset contains limited customer information. Segmentation performance can be improved by including additional features such as:

- Purchase history
- Product categories
- Visit frequency
- Average transaction value
- Loyalty membership details
- Mobile application usage
- Online shopping behavior
- Customer feedback and satisfaction ratings

These additional behavioral features would enable more accurate and personalized customer segmentation.

---

# ✅ Conclusion

This project successfully demonstrated how **Unsupervised Machine Learning** can be used to discover hidden customer segments in retail data.

Three clustering algorithms—**K-Means**, **Agglomerative Clustering**, and **DBSCAN**—were implemented, evaluated, and compared using multiple clustering validation metrics.

Among these, **K-Means Clustering** provided the best balance of clustering quality, computational efficiency, stability, and business interpretability. The resulting customer personas can support data-driven marketing strategies, improve customer satisfaction, and increase business profitability.

The project highlights the practical value of customer segmentation in retail analytics and provides a scalable foundation for future recommendation systems and personalized marketing applications.

---

# 👩‍💻 Author

**Sanika Kale**

MCA Student | Data Analytics & Machine Learning

Red & White Skill Education






































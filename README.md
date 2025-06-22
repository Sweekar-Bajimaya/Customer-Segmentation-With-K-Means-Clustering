# 🧠 Customer Segmentation with K-Means Clustering

This project applies **unsupervised machine learning** to segment customers based on their purchasing behavior using **K-Means Clustering** and **PCA for visualization**. The analysis helps businesses target specific customer groups more effectively by understanding how they shop across web, store, and catalog channels.

---

## 📌 Project Objective

Segment customers from a marketing campaign dataset to:
- Understand customer behavior across different shopping channels
- Identify distinct customer types for targeted marketing
- Recommend business strategies based on customer clusters

---

## 🧰 Tools & Technologies

- Python 3.x
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn
- PCA (Principal Component Analysis)
- K-Means Clustering

---

## 📁 Dataset Description

Dataset used: `marketing_campaign.csv`

### 📘 Feature Dictionary
| Feature | Description |
|--------|-------------|
| `NumDealsPurchases` | Purchases made with discount deals |
| `NumWebPurchases` | Purchases made via website |
| `NumCatalogPurchases` | Purchases made via catalog |
| `NumStorePurchases` | Purchases made in store |
| `NumWebVisitsMonth` | Monthly website visit frequency |

These features represent customer behavior across multiple purchase channels and are used to define cluster segments.

---

## 🧪 Process Overview

1. **Data Cleaning**
   - Removed nulls, normalized values, and selected behavioral features
2. **Feature Scaling**
   - Standardized features using `StandardScaler`
3. **Optimal Clustering**
   - Used **Elbow Method** to determine the best number of clusters (k=3)
4. **Modeling**
   - Applied **K-Means Clustering** and assigned cluster labels
5. **Visualization**
   - Reduced dimensionality using **PCA**
   - Visualized clusters and centroids in 2D space

---

## 📈 Visual Output

![image](https://github.com/user-attachments/assets/4c18b1d8-8081-4a66-8783-fbc03af6e99a)


> PCA plot showing 3 customer segments and their centroids

---

## 🧩 Key Insights

| Cluster | Behavior | Recommendation |
|--------|----------|----------------|
| Segment 0 | High purchases, especially online | Target with digital campaigns and loyalty offers |
| Segment 1 | High web visits, low purchase | Engage with personalized offers or retargeting |
| Segment 2 | High catalog/store purchases | Focus on traditional marketing (catalogs, in-store) |

---

## ✅ Business Recommendations

- **Segment 0**: Leverage for online promotions and exclusive deals
- **Segment 1**: Nurture with incentive-based campaigns to drive conversions
- **Segment 2**: Invest in offline marketing like catalogs and store coupons

---

## 📂 Project Structure
Customer-Segmentation-KMeans/
├── customer_segmentation.ipynb
├── README.md

---

## 📌 Future Enhancements
- Add silhouette score or Davies-Bouldin index for cluster validation
- Build an interactive dashboard using Streamlit or Dash
- Extend to RFM-based segmentation or customer lifetime value modeling


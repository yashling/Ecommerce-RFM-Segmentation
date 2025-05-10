# 🛒 RFM Customer Segmentation – eCommerce Orders Analysis

This project leverages the **RFM (Recency, Frequency, Monetary)** model to perform customer segmentation using an eCommerce dataset. The goal is to identify distinct customer groups based on purchasing behavior and help businesses tailor marketing strategies for each segment.

![Customer Segmentation Visualization](b3f920a9-b1ca-40b4-b0c1-eaa2e97af032.png) <!-- Add your segmentation chart here -->

---

## 📦 Dataset

- **Source**: Kaggle
- **Records**: 30,000+ transactions
- **Fields Used**: `user_id`, `created_at`, `total`, `order_id`

---

## 🔍 Project Highlights

- Cleaned and preprocessed the transactional dataset (date conversion, null handling)
- Calculated **RFM scores**:
  - **Recency**: Days since last purchase
  - **Frequency**: Number of orders
  - **Monetary**: Total spend
- Assigned RFM score segments using quantiles
- Created customer clusters using **KMeans** clustering
- Visualized clusters with count plots and spending distributions

---

## 🔢 RFM Table Sample

| Customer | Recency | Frequency | Monetary | RFM Score | Segment     |
|----------|---------|-----------|----------|-----------|-------------|
| 7337     | 12      | 5         | \$1520   | 444       | Champions   |
| 4868     | 89      | 1         | \$1771   | 211       | New Customers |
| 4337     | 37      | 3         | \$2567   | 332       | Potential Loyalists |

---

## 🧰 Tech Stack

- **Python 3**
- `pandas`, `datetime`, `seaborn`, `matplotlib`
- `sklearn` (for KMeans clustering)
- `numpy`

---

## 📈 Visualizations

- RFM distribution histograms
![RFM distribution histograms](e0ab9fe8-5330-4ec3-8b28-fefdd43a88d9.png)
- Elbow Method & Silhouette Score Analysis
![Elbow Method & Silhouette Score Analysis](6300d323-79ce-49d7-9c55-60685f406b82.png)
- Customer clusters based on RFM scores
![Customer clusters based on RFM scores](a511c5a5-d94a-4399-a5ad-035fffed6c38.png)
- DBSCAN Clustering (Anomaly Detection)
![DBSCAN Clustering (Anomaly Detection)](ea973abf-6603-4d1d-acfc-ef80542ed88c.png)



---

## 🧪 How to Run the Notebook

1. Clone the repo:
```bash
git clone https://github.com/yashling/Ecommerce-RFM-Segmentation.git
cd Ecommerce-RFM-Segmentation
jupyter notebook RFM_Customer_Segmentation.ipynb

# 🧩 Credit Card Customer Segmentation (Clustering Project)

### 📊 Dataset
**Source:** [Credit Card Dataset for Clustering (Kaggle)](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)

This project segments credit card customers based on their **spending patterns**, **repayment behavior**, and **credit usage** — using **unsupervised machine learning**.

---

## 🎯 Objective

To group customers into meaningful segments such as:
- 💳 *Revolver Customers* (cash-advance heavy)
- 💤 *Occasional Customers* (low engagement)
- 🏆 *Premium Customers* (high-spending, disciplined)
- ⚖️ *Moderate Customers* (average spenders with mixed cash use)

---

## 🧠 Techniques Used

| Step | Description |
|------|--------------|
| 1️⃣ Problem Definition | Identify behavioral segments from financial data |
| 2️⃣ Data Cleaning | Handle missing values and drop unnecessary columns |
| 3️⃣ EDA | Explore purchase & cash advance behavior |
| 4️⃣ Scaling | Standardize features using `StandardScaler` |
| 5️⃣ Dimensionality Reduction | Use PCA for 2D visualization |
| 6️⃣ Clustering | Apply KMeans and Agglomerative Clustering |
| 7️⃣ Evaluation | Elbow Method + Silhouette Score |
| 8️⃣ Interpretation | Label clusters based on behavioral traits |
| 9️⃣ Model Saving | Save trained model with `joblib` |

---

## 🧩 Key Insights

| Cluster | Label | Key Traits |
|----------|--------|------------|
| 0 | 💸 **Revolver Customers** | High balance & cash advance usage; low full payment rate |
| 1 | 💤 **Occasional Customers** | Low balance, low activity, small irregular purchases |
| 2 | 🏆 **Premium Customers** | High purchases, high frequency, regular payments |
| 3 | ⚖️ **Moderate Customers** | Moderate balance, occasional cash use, low payment ratio |

---

## 📈 Visualizations

- PCA Projection (2D customer space)
- Cluster distribution bar chart
- Elbow and Silhouette analysis

---

## 🧮 Evaluation
| Model | Silhouette Score |
|--------|------------------|
| **KMeans** | 0.166 |
| **Agglomerative** | 0.154 |

K-Means provided slightly more consistent and interpretable clusters.

---

## 💾 Files Included

| File | Description |
|------|--------------|
| `CreditCardCustomer_clustering.ipynb` | Jupyter notebook with full workflow |
| `customer_segmentation_model.pkl` | Saved trained clustering model |
| `README.md` | Project documentation |
| `requirements.txt` | Python dependencies |

---

## ⚙️ Installation & Run

```bash
git clone https://github.com/<yourusername>/CreditCardCustomer_Clustering.git
cd CreditCardCustomer_Clustering
pip install -r requirements.txt
jupyter notebook CreditCardCustomer_clustering.ipynb

🧰 Requirements

nginx
Copy code
pandas
numpy
matplotlib
seaborn
scikit-learn
joblib

🧭 Future Enhancements

Add DBSCAN for density-based comparison
Build dashboard using Streamlit for interactive visualization
Deploy model as an API

👤 Author
SONIA FIRDOUS
📧 soniafirdous1985@gmail.com


# Data-Science-Project
Customer Segmentation 

# 💡 Customer Segmentation App (Streamlit + Machine Learning)

## 📌 Overview
This project is a **Customer Segmentation Web App** built using **Machine Learning (K-Means Clustering)** and **Streamlit**.
It predicts the **customer segment (cluster)** based on user input such as income, spending, and purchase behavior.
This helps businesses understand customer groups and make better marketing decisions.

## 🚀 Features
* 📊 Predict customer segment using ML model
* 🎯 Uses K-Means clustering for segmentation
* ⚡ Real-time prediction via Streamlit UI
* 📈 Based on customer behavior data
* 🧠 Uses trained model (`kmeans_model.pkl`)
* 🔄 Scaled input using `StandardScaler`

## 🧠 Machine Learning Approach

* Algorithm Used: **K-Means Clustering**
* Preprocessing:

  * Feature Scaling using `StandardScaler`
* Features used:

  * Age
  * Income
  * Total Spending
  * Number of Web Purchases
  * Number of Store Purchases
  * Number of Web Visits
  * Recency

## 🏗️ Project Structure

Customer-Segmentation/
│
├── segmentation.py        # Streamlit app
├── kmeans_model.pkl       # Trained KMeans model
├── scaler.pkl             # Scaler used for preprocessing
├── customer_segmentation.csv  # Dataset
├── Analysis_Model.ipynb   # Model training notebook
└── README.md

## ⚙️ Installation

### Step 1: Clone the repository

```
git clone https://github.com/your-username/customer-segmentation.git
cd customer-segmentation
```

### Step 2: Install dependencies

```
pip install -r requirements.txt
```

If you don’t have requirements.txt, install manually:

```
pip install streamlit pandas numpy scikit-learn joblib
```

---

## ▶️ Run the App

```
streamlit run segmentation.py
```

Then open in browser:

```
http://localhost:8502
```

---

## 📸 Application Preview

*(Add your screenshot here)*

---

## 📊 How It Works

1. User enters customer details
2. Input data is converted into a DataFrame
3. Data is scaled using `StandardScaler`
4. KMeans model predicts cluster
5. Result is displayed on UI

## 🎯 Output

The model predicts:

👉 **Customer Segment (Cluster Number)**

Example:

```
Cluster 0 → Low Spending Customers  
Cluster 1 → Medium Spending Customers  
Cluster 2 → High Value Customers  
```

---

## ⚠️ Important Note

* Feature names during prediction must match training data
* Model is unsupervised (no labels required)
* Results depend on training dataset

---

## 🔮 Future Enhancements

* Add cluster visualization (graphs)
* Display customer segment meaning clearly
* Deploy on Streamlit Cloud / Render
* Integrate with chatbot (AI Financial Advisor)
* Add multilingual support

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Streamlit
* Joblib

## 👩‍💻 Author

**Vandana D L**
CSE Student | Data Science Enthusiast


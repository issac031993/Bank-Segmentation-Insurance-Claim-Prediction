# 🏦 Customer Segmentation & Insurance Claim Prediction

👋 **Hi, I'm Issac Abraham.**
This repository contains two comprehensive data mining projects I completed independently, applying clustering for customer segmentation and machine learning models to predict insurance claims.

---

## 🚀 Project Summary
📈 **Repo:** `Customer-Segmentation-Claim-Prediction`

This project has two main parts:

1. **Customer Segmentation:**  
   For a bank, identified customer groups based on credit card usage to drive promotional offers.

2. **Insurance Claim Prediction:**  
   For an insurance firm, built models to predict claim status using CART, Random Forest, and ANN.

---

## 🔍 Part 1: Clustering Analysis for Bank Customers

### 🏦 Business Context
A bank wanted to segment its customers to target promotions effectively. Data included:
- Spending, advance payments, credit limit, current balance, min payments, max single spend, probability of full payment.

### 📊 Approach & Findings
- **EDA:**  
  - No missing data.  
  - Spending & advance payments are positively skewed, with few outliers.
  - Strong positive correlations among spending, advance payments, credit limit.

- **Scaling:** Used StandardScaler to normalize features for clustering.

- **Clustering Techniques:**
  - **Hierarchical Clustering:** Dendrograms (Ward’s & Average) showed optimal clusters at **3**, confirmed by `fcluster` frequencies.
  - **K-Means Clustering:**  
    - Elbow curve & silhouette score also suggested **3 clusters**.
    - Clusters interpreted as **High / Medium / Low spenders**.

### 💼 Business Recommendations
| Segment | Strategy |
|---------|----------|
| **High Spend** | Offer reward points, increase credit limit, tie-ups with luxury brands. |
| **Medium Spend** | Promote premium cards & loyalty programs, target travel/e-commerce partnerships. |
| **Low Spend** | Encourage spending with grocery/utilities partnerships, reminders for payments.|

---

## 📊 Part 2: Insurance Claim Prediction using CART, RF, ANN

### 🛡 Business Context
An insurance company providing tour insurance wanted to predict claim status to better manage costs & marketing.

- **Features:** Age, agency code, product type, channel (online/offline), destination, sales, commission, duration.

### 🔍 Approach
- Performed extensive **EDA & outlier checks** on sales, age, commission, duration.
- Used MinMaxScaler for ANN models.

### 🧠 Models Compared
| Model               | Train Accuracy | Test Accuracy | AUC |
|----------------------|----------------|---------------|-----|
| **Decision Tree (CART)** | ~80% | ~78% | Visual ROC |
| **Random Forest**    | Best performance | ~80% | Highest ROC |
| **ANN (MLP)**        | Slightly lower | ~75% | Moderate ROC |

✅ **Conclusion:**  
- **Random Forest** consistently outperformed CART & ANN on accuracy, precision, recall, and F1.

---

## 💡 Business Recommendations
- Focus on **optimizing online channels**, which account for 90% of policies.
- Train underperforming agencies (like JZI) or explore partnerships with alternate agencies.
- Cross-sell insurance during flight/hotel booking, based on identified claim patterns.
- Use model outputs to prioritize claim verifications, combat fraud, and improve customer experience.

---

## 📈 Key Visualizations
- 📊 Clustering dendrograms & KMeans elbow plots
- ![Dendogram1](https://github.com/user-attachments/assets/0e32cd70-8dc8-4a63-a174-0a7f2ec14f15)

![ROC](https://github.com/user-attachments/assets/288c32f2-930a-4725-a563-26872ef834de)
- ![image](https://github.com/user-attachments/assets/7cde5283-815d-4543-902b-9cac9dfcb193)

- 🚦 Confusion matrices, ROC curves for CART, RF, ANN
- Please refer the pictures for complete images and analysis. 

---

## 🛠️ Tools & Skills Covered
- 🐍 Python: pandas, numpy, seaborn, matplotlib, scikit-learn
- 📊 Data Mining: Clustering (Hierarchical, KMeans), Decision Trees, Random Forests, ANN
- 🔍 Model tuning (GridSearchCV), silhouette scores, ROC-AUC evaluations
- 📈 Business storytelling & actionable strategies

---

## ⚙️ How to Run
- Open `Problem 1 - data mining.ipynb` for clustering & segmentation.
- Open `Problem 2 - data mining.ipynb` for CART, RF & ANN claim prediction.

---

## 🤝 About Me
I completed this project end-to-end, showcasing robust skills in data preprocessing, machine learning, clustering, and delivering business-focused insights.

🔗 [LinkedIn](https://linkedin.com/in/yourprofile)

---

✅ **Thanks for exploring my customer segmentation & insurance analytics work!**

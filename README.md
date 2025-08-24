# 🏦 PRODIGY_DS_03 - Decision Tree Classifier (Bank Marketing Dataset)

## 📌 Project Overview
This project is part of my **Data Science Internship at Prodigy InfoTech**.  
The objective of **Task 03** is to build a **Decision Tree Classifier** that predicts whether a customer will purchase a product/service based on the **Bank Marketing Dataset**.

The dataset contains customer demographic, financial, and campaign-related information.  
By analyzing these features, we can model customer behavior and provide useful insights for targeted marketing.

---

## 📂 Dataset
We used a merged dataset (`bank.csv`) combining:
- **bank-full.csv** (original dataset, 45k records, 17 features)  
- **bank-additional-full.csv** (extended dataset, 41k records, 21 features)  

The merged dataset contains **86,399 records and 23 features**.  

- **Target Variable**: `y` → (yes/no) whether the customer subscribed.  
- **Features**:  
  - Demographics → `age`, `job`, `marital`, `education`  
  - Financial → `balance`, `housing`, `loan`  
  - Campaign → `contact`, `month`, `duration`, `campaign`, `pdays`, `previous`, `poutcome`  
  - Macroeconomic Indicators → `emp.var.rate`, `cons.price.idx`, `cons.conf.idx`, `euribor3m`, `nr.employed`

---

## ⚙️ Steps Performed
1. **Data Exploration**  
   - Checked dataset shape, columns, and missing values.  
   - Combined both datasets into a single cleaned dataset.  

2. **Data Preprocessing**  
   - Filled missing values (median for numeric, `"unknown"` for categorical).  
   - Applied **one-hot encoding** to categorical variables.  

3. **Model Building**  
   - Split dataset into training (80%) and testing (20%).  
   - Trained a **Decision Tree Classifier** (`max_depth=5`).  

4. **Evaluation**  
   - Accuracy Score  
   - Confusion Matrix  
   - Classification Report (Precision, Recall, F1-Score)  

5. **Visualization**  
   - Decision Tree Structure  
   - Confusion Matrix Heatmap  
   - Top 10 Feature Importances  

---

## 📊 Results
- **Model Accuracy**: ~ (depends on dataset, typically ~0.85-0.90)  
- **Most Important Features**:  
  - `duration` (call duration)  
  - `euribor3m` (economic indicator)  
  - `pdays` (previous contact days)  
  - `campaign` (number of contacts during campaign)  
  - `age`, `job`, `housing` loan status  

These insights suggest that **economic conditions** and **customer contact history** significantly influence marketing success.

---

## 🚀 Tools & Libraries
- **Language**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  

---

## 📌 How to Run
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/PRODIGY_DS_03.git
   cd PRODIGY_DS_03

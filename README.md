# 🎓 Student POR – Predicting Portuguese Students’ Performance  

📊 **Author:** Gianfranco Damiani  
🎓 Data Analyst & Data Science Student @ Start2Impact University  

---

## 🧭 Project Overview  
This project analyzes the **Student Performance Dataset** (Portuguese course) to explore academic patterns and build predictive models for students’ final grades (**G3**).  
The goal is to identify **key factors influencing academic performance** and design **data-driven strategies** to support students from disadvantaged backgrounds.  

**Tech stack:** Python, pandas, scikit-learn, matplotlib, seaborn  

---

## 🎯 Project Presentation  
![Slide 1](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/1.png?raw=true)
![Slide 2](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/2.png?raw=true)

---

## 🧾 Dataset Overview  
![Slide 3](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/3.png?raw=true)

**Source:** Student Performance Dataset (UCI Repository)  
**File used:** `student-por.csv` (Portuguese course)  
**Dimensions:** 649 students × 33 variables  

Key variables include:  
- 👨‍👩‍👧 Family & Social: parents’ education, occupation, family size  
- 🧍‍♂️ Personal & Behavioral: age, gender, outings, alcohol consumption  
- 📚 Academic: study time, absences, educational support  
- 🧾 Performance: G1, G2, G3 (grades for 1st, 2nd, 3rd period)  

---

## 🔍 Exploratory Data Analysis (EDA)  
![Slide 4](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/4.png?raw=true)

- Strong correlation between **G3** and previous grades (**G1**, **G2**)  
- Study time and parental education show positive impact  
- Failures and alcohol consumption negatively influence grades  

---

## ⚙️ Methodology  
![Slide 5](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/5.png?raw=true)

Steps:  
1️⃣ EDA – Analyze distributions, correlations, key variables  
2️⃣ Preprocessing – Imputation, scaling, one-hot encoding  
3️⃣ Scenarios – Predict **G3** with/without intermediate grades (G1, G2)  
4️⃣ Models – Linear Regression, Random Forest, SVR  
5️⃣ Validation – RandomizedSearchCV + Nested CV for robust tuning  
6️⃣ Evaluation – Metrics: MAE, RMSE, R²  
7️⃣ Interpretation – Permutation Importance  

---

## 🧠 Model Results  
![Slide 6](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/6.png?raw=true)

| Scenario | Model | RMSE | MAE | R² |
|-----------|--------|------|------|----|
| With G1/G2 | Random Forest | 1.21 | 0.73 | 0.85 |
| With G1/G2 | Linear Regression | 1.22 | 0.77 | 0.85 |
| Without G1/G2 | Random Forest | 2.79 | 2.02 | 0.20 |
| Without G1/G2 | Linear Regression | 2.86 | 2.16 | 0.16 |

**Random Forest** proved the most stable and reliable model.

---

## 📊 Feature Importance  
![Slide 7](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/7.png?raw=true)

Most influential features:  
- ❌ **Failures** → more failures = lower grades  
- ⏱️ **Study time** → more hours = better performance  
- 🍷 **Dalc/Walc** → alcohol use penalizes grades  
- 🎓 **Parental education** → higher education = higher achievement  
- 🚫 **Absences** → reduce performance  

---

## 💡 Insights & Strategies  
![Slide 8](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/8.png?raw=true)

Recommendations:  
- Implement tutoring for students with past failures  
- Promote healthy study habits and awareness on alcohol use  
- Monitor absences to reduce dropouts  
- Engage parents through educational programs  

---

## 📘 Jupyter Notebook  
👉 [Open Progetto Finale Data Science di Gianfranco Damiani.ipynb on GitHub](https://github.com/Gianfranco-rgb/-Student-POR-Predicting-Portuguese-Students-Performance/blob/main/Progetto%20Finale%20Data%20Science%20di%20Gianfranco%20Damiani.ipynb)

---

## 🧩 Key Takeaways  
- Built predictive models for academic success (Random Forest performed best)  
- Highlighted socio-academic variables impacting performance  
- Developed actionable strategies for educators and policymakers  

---

👨🏻‍💻 **Author:** [Gianfranco Damiani](https://github.com/Gianfranco-rgb)  
📧 [gianfranco.damiani@icloud.com](mailto:gianfranco.damiani@icloud.com)  
📍 Bologna / Madrid 🇮🇹🇪🇸  

# 🌾 KreditKisan — Dynamic Pricing Engine for Microloans

## 🚀 Overview

This project replaces traditional **flat interest rates (18%)** with a **machine learning–based dynamic pricing system**.

It predicts **personalized interest rates** for loan applicants based on their risk profile, improving:

* ✅ Profitability for lenders
* ✅ Fairness for borrowers
* ✅ Financial inclusion

---

## 🧠 Key Features

* 📊 Exploratory Data Analysis (EDA)
* 🤖 Gradient Boosting Regressor model
* ⚖️ Fairness analysis (Age & Business Type)
* 🧩 Risk tier segmentation (Low → Very High)
* 💻 Streamlit UI for real-time predictions
* 📈 Comparison with flat 18% pricing

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
* Streamlit

---

## 📂 Project Structure

```
Microloan_pricing_ETE/
│
├── app.py                  # Streamlit UI
├── main.py                 # ML pipeline (training + evaluation)
├── kreditkisan_model.pkl   # Trained model (generated after running main.py)
├── data.csv                # Dataset
├── outputs/                # Graphs & results
├── .gitignore
├── README.md
```

---

## ⚙️ Setup Instructions (Run Locally)

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/microloan-dynamic-pricing.git
cd microloan-dynamic-pricing
```

---

### 2️⃣ Create virtual environment

```bash
python -m venv venv
```

Activate:

**Windows:**

```bash
venv\Scripts\activate
```

---

### 3️⃣ Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn streamlit joblib
```

---

### 4️⃣ Train the model

```bash
python main.py
```

👉 This will:

* Train the ML model
* Generate graphs
* Save `kreditkisan_model.pkl`

---

### 5️⃣ Run the UI

```bash
python -m streamlit run app.py
```

👉 Open in browser:

```
http://localhost:8501
```

---

## 💡 How It Works

1. User enters applicant details
2. Model predicts interest rate
3. System assigns risk tier:

   * Low
   * Medium
   * High
   * Very High
4. UI shows:

   * Predicted rate
   * Risk classification
   * Comparison with flat 18%

---

## ⚖️ Fairness Consideration

The model is evaluated to ensure:

* No unfair bias across **Business Types**
* No unjustified disparity across **Age groups**

This ensures pricing is **risk-based, not discriminatory**.

---

## 📊 Business Impact

| Approach | Outcome                      |
| -------- | ---------------------------- |
| Flat 18% | Same rate for all            |
| ML Model | Higher profit + fair pricing |

✔ Low-risk → Lower rates (more inclusion)
✔ High-risk → Higher rates (risk-adjusted profit)

---

## 👥 Team Roles

* ML Engineer — Model building & training
* Data Analyst — EDA & insights
* Business Analyst — Risk tiers & fairness
* Presenter — PPT & demo
* Code Reviewer — Integration & UI

---

## 🎯 Future Improvements

* Deploy online (Streamlit Cloud / Render)
* Add loan approval system
* Improve explainability (SHAP values)
* Add user authentication

---

## 📌 Note

Make sure:

* `data.csv` is present before running
* Model file (`.pkl`) is generated before starting UI

---

## 🏁 Conclusion

This project demonstrates how **AI can transform lending** by making it:

* Smarter
* Fairer
* More profitable

---

**Built for learning, impact, and real-world fintech applications 🚀**

# 🛠 Customer Support Analytics: Satisfaction & Resolution Time Prediction

This project is an end-to-end ML solution that analyzes customer support tickets to predict customer satisfaction (classification) and resolution time (regression). Built with a user-friendly Streamlit interface, it allows users to upload CSVs, perform exploratory analysis, and generate predictions.

---

## 📌 Overview

The application ingests customer support ticket data, preprocesses it with rich feature engineering, and applies trained ML models to:

- Predict whether the customer will be **satisfied or unsatisfied**
- Estimate the **expected time to resolve** the support request

---

## 🚀 Features

* Classifies support satisfaction using an ensemble Voting Classifier
* Predicts resolution time using Linear Regression
* Extracts 290+ features using sentiment analysis (VADER, TextBlob), TF-IDF, and ticket metadata
* Visualizes data distribution, feature importance, and model results in Streamlit
* Interactive CSV upload with per-ticket insights

---

## 🛠️ Technologies Used

* Python
* Scikit-learn
* TextBlob & VADER
* Pandas & NumPy
* Streamlit
* Matplotlib & Seaborn
* Jupyter Notebook

---

## 🧠 Model Details

### Satisfaction Prediction:
* Model: Voting Classifier (Logistic Regression + Decision Tree + Random Forest)
* Metric: F1 Score – **56.3%**
* Features: Sentiment polarity, ticket urgency, TF-IDF vectors, categorical encodings

### Resolution Time Prediction:
* Model: Linear Regression
* Metric: MAE – **0.077 hours**, RMSE ~0.0106
* Notes: Temporal, categorical, and text features combined for high accuracy

---

## 📷 Streamlit Preview

<img width="1917" height="913" alt="image" src="https://github.com/user-attachments/assets/a80e8afd-4b0b-4650-87c4-4a4dbaaad83a" />
<!-- Replace or remove this if not available -->

---

## 📦 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/kkrishnateja/Customer-Experience-Analytics-Sentiment-and-Resolution-Prediction.git
   cd Customer-Experience-Analytics-Sentiment-and-Resolution-Prediction
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

---

## 📁 Project Structure

```
Customer-Experience-Analytics-Sentiment-and-Resolution-Prediction/
├── app/
│   └── app.py                  # Streamlit interface
├── models/
│   ├── satisfaction_model.pkl  # Voting Classifier
│   └── time_model.pkl          # Linear Regression
├── utils/
│   └── preprocessing.py        # Feature engineering & encoding
├── data/
│   └── sample_tickets.csv      # Example support data
├── requirements.txt
├── README.md
└── model.ipynb      # Full pipeline development

```

---

## 📄 License

This project is for educational use only.

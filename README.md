# Finance_Complaints
# 📝 Finance Complaint Classification - ML & App Deployment

A Machine Learning project to classify consumer financial complaints into predefined product categories. It uses NLP (TF-IDF + Logistic Regression) and provides both an **API (FastAPI)** and **Web App (Streamlit)** for real-time predictions.

---

## 📌 Project Overview

Consumers often lodge complaints related to banking, loans, credit cards, and other financial services. Manually handling these is time-consuming. This project builds an automated system to:

- Clean complaint texts
- Extract features using TF-IDF
- Train and evaluate classification models
- Deploy the model using FastAPI & Streamlit
- Provide rich visual insights using Python visual libraries

---

## 📂 Dataset

- 📁 Source: [Consumer Financial Protection Bureau - Public Complaint Database](https://www.consumerfinance.gov/data-research/consumer-complaints/)
- Format: `.csv` (columns include Product, Complaint Narrative, Date, etc.)

---

## 🧰 Features

- TF-IDF vectorization for NLP feature extraction
- Logistic Regression classifier (customizable to others: SVM, XGBoost)
- Modular code: separate model, API, and app layers
- Data visualization: WordCloud, Plotly, Seaborn
- Deployment-ready with FastAPI (REST API) and Streamlit (UI)

---

## 🏗️ Project Structure

finance_complaint_classifier/
├── app/
│ ├── main.py # FastAPI app
│ ├── streamlit_app.py # Streamlit UI app
│ └── model/
│ ├── complaint_classifier.pkl
│ └── tfidf_vectorizer.pkl
├── data/
│ └── complaints.csv
├── notebook/
│ └── Finance_Complaints_Classifier.ipynb
├── requirements.txt
└── README.md
---

## 🚀 How to Run

### ⚙️ Environment Setup

```bash
git clone https://github.com/your-username/finance-complaint-classifier.git
cd finance-complaint-classifier
pip install -r requirements.txt
```

##Jupyter Notebook (Training + EDA)
jupyter notebook notebook/Finance_Complaints_Classifier.ipynb

##Visualizations Included
Bar chart of top complaint categories

Word Cloud of complaint narratives

Boxplot of complaint lengths

Interactive Plotly trend analysis

TF-IDF keyword insights (optional)

<p align="center"> <img src="https://user-images.githubusercontent.com/example/bar_chart.png" width="500"/> <img src="https://user-images.githubusercontent.com/example/wordcloud.png" width="500"/> </p>

##Future Improvements
Use advanced NLP models (BERT, RoBERTa)

Add label explanation (e.g., via SHAP)

Active learning or feedback loop from users

CI/CD with Docker, GitHub Actions

Cloud deployment (AWS/GCP/Azure)


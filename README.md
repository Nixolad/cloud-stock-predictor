# ☁️ Tomorrow’s Stock Predictor – Cloud SaaS Project

This repository contains a **cloud-based stock prediction platform** and an associated **machine learning research subproject**. Together, they form a complete demonstration of building, evaluating, and deploying stock prediction models in a scalable, cloud-hosted environment.

---

## 📊 Project Overview

**Main Project:**  
**Cloud-Based Stock Prediction Web Application**  
A lightweight SaaS app where users can search for a stock ticker, view live price trends, and get an **AI-generated prediction** of whether the stock will move **up or down tomorrow**.

**Subproject:**  
**Assessment of Simple Supervised Learning Models**  
An experimental study of several baseline ML techniques (Linear Regression, Logistic Regression, SVM, KNN, Neural Network) applied to tomorrow’s stock direction classification.

Both projects are interlinked — the best-performing model from the research phase will be deployed to the cloud app.

---

## 🧠 Subproject 1: ML Model Evaluation

Located in: [`model_research/`](model_research/)

This part of the project explores:
- Fetching and preparing historical stock data using `yfinance`.
- Creating a **classification label**: {up, down, stay} based on daily price movements.
- Applying **PCA (Principal Component Analysis)** for dimensionality reduction.
- Comparing multiple supervised learning models.

The primary goal: achieve better-than-random prediction performance while demonstrating clear ML workflow steps.

---

## ☁️ Subproject 2: Cloud SaaS Application

Located in: [`cloud_app/`](cloud_app/)

This is a simple full-stack cloud deployment that includes:
- **Frontend:** A web interface for users to log in and check predictions.
- **Backend:** Python API (Flask/FastAPI) serving predictions from the trained ML model.
- **Cloud Infrastructure:** Google Cloud Run, Cloud SQL, and Cloud Storage.

Expected features:
- User registration & authentication  
- Stock ticker search  
- Real-time stock display  
- AI-generated next-day prediction

---

## 🏗️ Architecture Overview
User -> Web Interface -> Backend API -> ML Model -> Cloud Services

Cloud SQL (user data) + Cloud Storage (model) -> User


---

## 🧩 Tech Stack

| Layer | Tools / Services |
|-------|------------------|
| Data | `yfinance`, `pandas`, `numpy` |
| ML | `scikit-learn`, `tensorflow` (optional) |
| API | `FastAPI` or `Flask` |
| Frontend | `HTML`, `CSS`, `JavaScript` |
| Cloud | Google Cloud Run, Cloud SQL, Cloud Storage |
| Version Control | GitHub |

---

## 🚧 Project Status

🟡 **Early Development (as of Nov 2025)**  
Data collection, feature engineering, and initial model experimentation are in progress.  
Cloud deployment will begin in **early December 2025**.

Follow progress via the `dev` branch and the `/docs` folder for updated architecture diagrams.

---

## 🔜 Future Work

- Evaluate additional ML models (e.g., Random Forest, LSTM)
- Integrate continuous data refresh with the cloud backend
- Add user portfolio tracking
- Deploy a minimal demo version for public access

---

## 📄 References

- [Rouf et al. (2021)] “Stock market prediction using machine learning techniques: a decade survey on methodologies, recent developments, and future directions.” *Electronics, 10(21), 2717.*
- [Usmani et al. (2016)] “Stock market prediction using machine learning techniques.” *IEEE ICCOINS.*

---

## 👤 Author

**Nick Karlman**  
📅 Started: November 2025  
📍 Hosted on: [GitHub](https://github.com/)  
💡 Aim: To integrate ML research and cloud deployment into a cohesive SaaS product.


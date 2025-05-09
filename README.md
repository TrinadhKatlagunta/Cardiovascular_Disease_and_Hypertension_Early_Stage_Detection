# Cardiovascular Disease and Hypertension Early Stage Detection

This repository contains two machine learning pipelines for predicting **Cardiovascular Disease (CVD)** and **Hypertension** at an early stage using multiple machine learning and deep learning models. The final selected models are **Decision Tree Classifiers (DTC)** for both pipelines, based on their performance and simplicity for deployment.

## 🌐 Live Demo

👉 [Deployed Web Application (on Render)](https://early-stage-cardio-vascular-disease.onrender.com/)

---

## 🧠 Project Overview

The goal of this project is to build intelligent systems that can assist in the **early diagnosis** of cardiovascular and hypertension-related health risks. Using medical records and health indicators, the models predict whether a patient is at risk or not.

---

## 📁 Directory Structure

```
CVD(Model Chaining)/
│
├── Cardio_Vascular_Disease_Detection_Main.ipynb # Notebook for CVD modeling & evaluation
├── Early_Stage_Detection_of_Hypertension.ipynb # Notebook for Hypertension modeling & evaluation
├── model/ # Saved model pickles for both pipelines
│ ├── dt_model_cvd.pkl
│ └── dt_model_hyp.pkl
├── static/ # Static files (CSS)
│ └── style.css
├── templates/ # HTML templates for Flask app
│ ├── home.html
│ ├── prediction.html
│ └── result.html
├── app.py # Flask backend app
└── requirements.txt # Python dependencies

```

## 📊 Machine Learning Models Tried

For both datasets (CVD and Hypertension), we experimented with a wide range of models:

### ✅ Classical ML Models

1. Logistic Regression  
2. Support Vector Classifier (SVC)  
3. Random Forest Classifier  
4. Decision Tree Classifier ✅ *(Final Selected)*  
5. K-Nearest Neighbors (KNN)  
6. Gaussian Naive Bayes  
7. Stochastic Gradient Descent Classifier  
8. AdaBoost Classifier  
9. Gradient Boosting Classifier  
10. Ridge Classifier  
11. Extra Trees Classifier  
12. Bagging Classifier  
13. Logistic Regression CV  
14. Voting Classifier  

### 🤖 Deep Learning Models

1. Artificial Neural Network (ANN)  
2. GRU (Gated Recurrent Unit)  
3. Bi-LSTM (Bidirectional Long Short-Term Memory)  
4. Custom BiLSTM Architectures  

---

## ✅ Final Model Selection

After rigorous evaluation using metrics like **accuracy**, **precision**, **recall**, and **loss curves**, we finalized the following models:

- 📌 **CVD Prediction** → Decision Tree Classifier  
- 📌 **Hypertension Prediction** → Decision Tree Classifier  

These were chosen for their high validation accuracy, low complexity, and strong interpretability — making them suitable for deployment.

---

## 🚀 Deployment

- ⚙️ Backend Framework: Flask  
- 🎨 Frontend: HTML, CSS (with Jinja templating)  
- 🌐 Deployment Platform: Render  

---

## ⚙️ Installation

To run this project locally:

```bash
git clone https://github.com/your-username/CVD-Hypertension-Detection.git
cd CVD-Hypertension-Detection
pip install -r requirements.txt
python app.py

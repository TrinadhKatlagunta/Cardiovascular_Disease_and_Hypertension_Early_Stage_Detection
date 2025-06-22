# Cardiovascular Disease and Hypertension Early Stage Detection

This repository contains two machine learning pipelines for predicting Cardiovascular Disease (CVD) and Hypertension at an early stage using multiple machine learning and deep learning models. The final selected models are Support Vector Classifier (SVC) for CVD prediction and Decision Tree Classifier (DTC) for Hypertension stage prediction, based on their performance and simplicity for deployment. The models achieved approximately 90% and 99% accuracy on their respective validation datasets.

## 🌐 Live Demo

👉 [Deployed Web Application (on Render)](https://early-stage-cardio-vascular-disease.onrender.com/)

## 🧠 Project Overview

The goal of this project is to build intelligent systems that can assist in the **early diagnosis** of cardiovascular and hypertension-related health risks. Using medical records and health indicators, the models predict whether a patient is at risk or not.

## 📁 Directory Structure

```
CVD(Model Chaining)/
│
├── Cardio_Vascular_Disease_Detection_Main.ipynb # Notebook for CVD modeling & evaluation
├── Early_Stage_Detection_of_Hypertension.ipynb # Notebook for Hypertension modeling & evaluation
├── models/ # Saved model pickles for both pipelines
│   ├── svm90.pkl
│   ├── standard_scaler.pkl
│   ├── dtc.pkl
│   └── minmax.pkl
├── static/ # Static files (CSS)
│   └── style.css
├── templates/ # HTML templates for Flask app
│   ├── index.html
├── app.py # Flask backend app
└── requirements.txt # Python dependencies
```

## 🧪 Models Explored

For both datasets (CVD and Hypertension), we experimented with a wide range of models:

### ✅ Classical Machine Learning Models

1. Logistic Regression  
2. Support Vector Classifier (SVC)  
3. Random Forest Classifier  
4. Decision Tree Classifier
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

### ✅ Deep Learning Models

1. Artificial Neural Network (ANN)  
2. GRU (Gated Recurrent Unit)  
3. Bi-LSTM (Bidirectional Long Short-Term Memory)  
4. Custom Bi-LSTM
5. ANN (Prime Anarchist) – a custom ANN model specifically built for hypertension stage prediction

## ✅ Final Model Selection

After evaluating multiple models using metrics like **accuracy**, **precision**, **recall**, and **loss curves**, we finalized the following:

- 📌 **CVD Prediction** → Support Vector Classifier (~90% accuracy)  
- 📌 **Hypertension Prediction** → Decision Tree Classifier (~99% accuracy)  

These models were selected for their high accuracy, simplicity, and interpretability — making them ideal for real-time deployment.

## 🚀 Deployment

- Web app built using **Flask**.
- Hosted on **Render**.
- Accepts user medical details and returns both **CVD risk prediction** and **Hypertension Stage** instantly.

## ⚙️ Installation

To run this project locally:

```bash
# Step 1: Clone the repository
git clone https://github.com/TrinadhKatlagunta/Cardiovascular_Disease_and_Hypertension_Early_Stage_Detection.git
cd Cardiovascular_Disease_and_Hypertension_Early_Stage_Detection

# Step 2: Create and activate virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Step 3: Install dependencies
pip install -r requirements.txt

# Step 4: Run the app
python app.py
```

## 👨‍💻 Team Members

- 👨‍🔬 **Sai Vidith** – Experimented with 14 ML & 4 DL models for optimal performance  
- 🧑‍💻 **Sandeep Rao** – Led data preprocessing and feature engineering  
- 🛠 **Phanindra** – Handled metric evaluation and ML pipeline testing  
- 🚀 **Trinadh Katlagunta** – Built model chaining, Flask integration, and full deployment  

> 🏫 B.Tech CSE (AI & ML) | R.V.R & J.C College of Engineering

## 📜 License

This project is open-source and free to use under the MIT License.

🩺 Diabetes Prediction using Support Vector Machine (SVM)
📌 Project Overview

This project implements a Support Vector Machine (SVM) model to predict whether a person is diabetic based on medical diagnostic measurements. The goal is to build an accurate classification model and evaluate its performance using standard machine learning metrics.

The dataset used is the Pima Indians Diabetes Dataset, a well-known benchmark dataset for binary classification problems.

🧠 Problem Statement

Diabetes is a chronic disease that requires early detection for effective treatment.
Using patient health parameters, this project predicts:

0 → Non-Diabetic

1 → Diabetic

📂 Dataset Information

Source: Pima Indians Diabetes Dataset (UCI / Kaggle)

Features:

Pregnancies

Glucose

BloodPressure

SkinThickness

Insulin

BMI

DiabetesPedigreeFunction

Age

Target:

Outcome (0 or 1)

⚙️ Technologies Used

Python

NumPy

Pandas

Matplotlib / Seaborn

Scikit-learn

🔍 Methodology

Data Loading & Exploration

Checked shape, missing values, and class distribution.

Data Preprocessing

Feature scaling using StandardScaler

Train-test split

Model Building

Implemented Support Vector Machine (SVM) classifier

Used linear / RBF kernel (depending on implementation)

Model Evaluation

Accuracy score

Confusion matrix

Classification report

📊 Results

Achieved good classification accuracy on test data.

Model effectively distinguishes between diabetic and non-diabetic patients.

(You can update this section with your actual accuracy, e.g., “Accuracy: 78%”.)

🛠️ How to Run the Project

Clone the repository:

git clone https://github.com/your-username/diabetes-svm.git


Navigate to the project directory:

cd diabetes-svm


Install required libraries:

pip install -r requirements.txt


Run the notebook / script:

python svm_diabetes.py

📁 Project Structure
├── dataset/
│   └── diabetes.csv
├── svm_diabetes.py   (or notebook file)
├── README.md
└── requirements.txt

📌 Future Improvements

Hyperparameter tuning using GridSearchCV

Try other classifiers (Logistic Regression, Random Forest, KNN)

Deploy using Flask / Streamlit

Handle missing values more robustly

🤝 Acknowledgements

UCI Machine Learning Repository

Kaggle

Scikit-learn documentation

👤 Author

Paras Rajput
Computer Science Student | Data Analytics & Machine Learning Enthusiast

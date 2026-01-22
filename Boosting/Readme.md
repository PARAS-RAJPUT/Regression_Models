# 🎗️ Breast Cancer Prediction using AdaBoost
## 📌 Project Overview

This project implements the AdaBoost (Adaptive Boosting) algorithm to classify breast tumors as benign or malignant based on diagnostic features. The objective is to build a high-performance ensemble classifier and evaluate its accuracy on a real medical dataset.

The dataset used is the Breast Cancer Wisconsin (Diagnostic) Dataset, a widely used benchmark dataset for binary classification problems in healthcare.

## 🧠 Problem Statement

Breast cancer early detection is crucial for effective treatment and survival.
Using medical diagnostic measurements extracted from breast mass images, this project predicts:

0 → Benign (Non-cancerous)

1 → Malignant (Cancerous)

This is a supervised binary classification problem.

## 📂 Dataset Information

Source: UCI Machine Learning Repository / Scikit-learn Breast Cancer Dataset

Number of Samples: 569
Number of Features: 30

Features include:

Radius (mean, se, worst)

Texture

Perimeter

Area

Smoothness

Compactness

Concavity

Symmetry

Fractal dimension

Target:

Diagnosis (Benign / Malignant)

## ⚙️ Technologies Used

Python

NumPy

Pandas

Matplotlib / Seaborn

Scikit-learn

## 🔍 Methodology

Data Loading & Exploration

Loaded dataset from Scikit-learn

Analyzed class distribution and feature statistics

Data Preprocessing

Feature scaling using StandardScaler

Train-test split

Model Building

Implemented AdaBoostClassifier

Base estimator: Decision Tree (stump)

Tuned number of estimators and learning rate

Model Evaluation

Accuracy score

Confusion matrix

Classification report

ROC-AUC score (optional)

## 📊 Results

Achieved high classification accuracy on test data.

AdaBoost significantly improved performance compared to a single decision tree.

Model effectively distinguishes malignant and benign tumors.

(You can replace this with your actual results, e.g., Accuracy: 96%.)


## 📁 Project Structure

dataset/breast_cancer.csv — Dataset file (if externally provided)

adaboost_breast_cancer.py — Main Python script / notebook

README.md — Project documentation

requirements.txt — Python dependencies

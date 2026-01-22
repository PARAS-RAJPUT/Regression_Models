# 🍷 Wine Classification using Hierarchical Clustering
## 📌 Project Overview

This project applies Hierarchical Clustering to the Wine Dataset to explore natural groupings of wines based on their chemical properties. The objective is to identify clusters of similar wines and visualize the clustering structure using dendrograms.

The Wine dataset is a classic benchmark dataset widely used for unsupervised learning and clustering tasks.

## 🧠 Problem Statement

Given multiple physicochemical attributes of wines, the task is to:

Group wines into meaningful clusters

Analyze similarities and differences between wine samples

Visualize hierarchical relationships using dendrograms

This is an unsupervised learning problem.

## 📂 Dataset Information

Source: UCI Machine Learning Repository / Scikit-learn Wine Dataset

Number of Samples: 178
Number of Features: 13

Features include:

Alcohol

Malic acid

Ash

Alcalinity of ash

Magnesium

Total phenols

Flavanoids

Nonflavanoid phenols

Proanthocyanins

Color intensity

Hue

OD280/OD315 of diluted wines

Proline

## ⚙️ Technologies Used

Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

SciPy

## 🔍 Methodology

Data Loading & Exploration

Loaded wine dataset

Checked shape, summary statistics, and correlations

Data Preprocessing

Feature scaling using StandardScaler

Removed class labels (unsupervised learning)

Hierarchical Clustering

Used Agglomerative Clustering

Distance metrics: Euclidean

Linkage methods: Ward / Complete / Average

Visualization

Constructed dendrograms using SciPy

Visualized clusters using 2D projections

Cluster Evaluation

Analyzed number of clusters

Compared clustering with original wine classes (optional)

## 📊 Results

Successfully identified natural groupings among wine samples.

Dendrogram revealed clear hierarchical structure.

Clusters showed strong alignment with original wine classes.

(You can update this with your chosen number of clusters and observations.)

## 📁 Project Structure

├── dataset/
│   └── wine.csv   (if external)
├── hierarchical_wine.py  (or .ipynb)
├── README.md
└── requirements.txt


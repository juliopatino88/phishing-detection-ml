# Phishing Website Detection: Decision Trees & K-Means Clustering

## Overview
This project tackles **phishing website detection** using both supervised and unsupervised machine learning approaches. A Decision Tree classifier is trained to predict whether a website is legitimate or phishing, and K-Means clustering is used to discover natural groupings in the data without labels.

This is a two-part analysis completed as coursework for **DATA 430 (Machine Learning)** at the University of Maryland Global Campus.

## Business Problem
Phishing attacks remain one of the most common cybersecurity threats. Automated detection systems need to classify websites quickly and accurately based on observable features like URL structure, domain registration, and page content — without relying solely on blacklists that can't catch new threats.

## Dataset
- **Source:** [UCI Machine Learning Repository — Phishing Websites](https://archive.ics.uci.edu/ml/datasets/phishing+websites)
- **Size:** ~11,000 website records
- **Features:** 30 attributes covering URL-based, domain-based, and HTML/JavaScript-based features
- **Target:** Binary classification (phishing vs. legitimate)

## Methods

### Part 1: Decision Tree Classification (Supervised)
- Exploratory data analysis
- Decision tree classifier with hyperparameter tuning (max_depth: 3, 5, None)
- Train/test split evaluation
- Analysis of overfitting risk at different tree depths
- Feature importance ranking

### Part 2: K-Means Clustering (Unsupervised)
- K-Means clustering to discover natural groupings without using labels
- Elbow method for optimal cluster selection
- Comparison of cluster assignments vs. actual labels
- Analysis of what features drive cluster separation

## Key Findings
- Decision tree at **max_depth=5** provided the best balance between accuracy and generalization
- Unlimited depth (None) led to **overfitting** — high training accuracy but lower test performance
- K-Means clustering identified meaningful groupings that partially aligned with the phishing/legitimate labels
- **URL-based features** (SSL state, URL length, domain registration) were among the strongest predictors

## Tools & Libraries
- Python (pandas, NumPy, scikit-learn, matplotlib, seaborn)
- Jupyter Notebook

## Files
- `Assignment_3_Decision_Trees.ipynb` — Decision tree classification analysis
- `Assignment_4_KMeans_Clustering.ipynb` — K-Means clustering analysis

## Author
**Julio Patiño**
- [LinkedIn](https://www.linkedin.com/in/juliopatino88/)
- [GitHub](https://github.com/juliopatino88)

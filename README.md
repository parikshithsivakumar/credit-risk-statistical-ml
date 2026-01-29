📊 Credit Risk Prediction using PCA, Clustering & Bayesian Models
Home Credit Default Risk 
📌 Overview

This repository contains the implementation of a statistically validated and interpretable credit risk prediction framework built using the Home Credit Default Risk dataset.

The project integrates:

Principal Component Analysis (PCA) for dimensionality reduction

Hierarchical Clustering for borrower segmentation

ANOVA & Cronbach’s Alpha for statistical validation

Discriminant Analysis (LDA, QDA) and Bayesian Estimation (Gaussian Naïve Bayes) for transparent credit risk prediction

The goal is to move beyond black-box machine learning models and provide a regulator-friendly, explainable, and scalable credit scoring pipeline.

👥 Team

Team 4

Aditya Elango

Parikshith Sivakumar

B.Tech – Computer Science & Engineering
Amrita Vishwa Vidyapeetham, Bengaluru

📁 Repository Contents
.
├── Team_4_Code.ipynb        # Main project notebook
├── Dataset/                # Dataset directory (excluded from Git)
│   ├── application_data.csv
│   └── previous_application.csv
├── requirements.txt        # Python dependencies (pip)
├── environment.yml         # Conda environment (optional)
├── README.md               # Project documentation
├── LICENSE                 # License file
└── .gitignore              # Dataset and environment exclusions

📊 Dataset

Source: Home Credit Default Risk Dataset

Records: ~300,000 borrowers

Features: 100+ demographic, financial, and credit-history attributes

Target Variable: Loan Default (0 = Non-default, 1 = Default)

⚠️ Data Handling

The dataset is not included in this repository due to size constraints.

Download the dataset and place the files in the Dataset/ folder with the following names:

application_data.csv

previous_application.csv

If hosting externally (Kaggle / Google Drive / S3), provide a download script or link.

🧠 Methodology Summary

Data Preprocessing

Missing value handling, encoding, normalization

Dimensionality Reduction

PCA applied to remove multicollinearity

23 principal components retained (~90% variance)

Borrower Segmentation

Agglomerative hierarchical clustering in PCA space

Statistical Validation

One-way ANOVA for cluster significance

Cronbach’s Alpha for feature reliability

Supervised Risk Modeling

Linear Discriminant Analysis (LDA)

Quadratic Discriminant Analysis (QDA)

Logistic Regression (baseline)

Bayesian Estimation

Gaussian Naïve Bayes for probabilistic default scoring

⚙️ Setup Instructions
🔹 Using pip (Recommended)
python -m venv .venv
.\.venv\Scripts\activate   # Windows
# source .venv/bin/activate  # macOS / Linux
pip install -r requirements.txt

🔹 Using conda
conda env create -f environment.yml
conda activate team4_env

▶️ Running the Project

Ensure the dataset is placed inside the Dataset/ folder

Launch Jupyter Notebook:

jupyter notebook


Open and run:

Team_4_Code.ipynb


Execute cells sequentially to reproduce:

PCA analysis

Clustering & dendrograms

Statistical tests (ANOVA, Cronbach’s Alpha)

Model training & evaluation

Bayesian default probability estimation

📈 Outputs Generated

PCA scree plots and explained variance graphs

Hierarchical clustering dendrogram

Cluster profiling tables

ANOVA F-statistics and p-values

Confusion matrices & ROC curves

Borrower default probabilities

📝 Notes

The notebook contains Colab-specific cells (e.g., google.colab.files.upload()).

Remove or guard these cells when running locally.

Clear notebook outputs before committing:

jupyter nbconvert --clear-output Team_4_Code.ipynb


or use:

nbstripout Team_4_Code.ipynb

🚀 Key Contributions

Unified PCA → Clustering → Statistical Validation → Classification pipeline

Borrower segmentation with statistical justification

Interpretable discriminant functions for credit scoring

Bayesian probabilistic risk estimation

Scalable and regulator-friendly design

🔮 Future Scope

Address class imbalance using SMOTE / ADASYN

Incorporate nonlinear embeddings (autoencoders, deep learning)

Explore advanced clustering methods (GMM, DBSCAN, HDBSCAN)

Deploy as a real-time credit scoring system

Extend validation across multiple financial datasets

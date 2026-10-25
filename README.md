###Week 3: Unsupervised Learning & Model Evaluation
Overview
This project explores unsupervised clustering and supervised model evaluation using the Breast Cancer Wisconsin dataset available in Scikit-learn.
Objectives
- Apply K-Means and Hierarchical Clustering.
- Explore cluster counts using the elbow method and silhouette scores.
- Use PCA for dimensionality reduction and cluster visualization.
- Evaluate a separate classification task using cross-validation, a confusion matrix, precision, recall, F1-score, and ROC-AUC.
- Tune Random Forest hyperparameters and compare results with Logistic Regression.
- Discuss feature selection, outliers, preprocessing choices, and model limitations.
Dataset
The dataset contains 569 observations and 30 numerical features describing cell-nucleus characteristics. Diagnosis labels are malignant and benign. The labels are not used to train clustering models; they are used in the separate classification experiment and for post-hoc cluster interpretation.
Methods
Unsupervised learning
- Inspect feature distributions and potential outliers using the IQR rule.
- Standardize features before distance-based clustering.
- Use the elbow method and silhouette scores to explore the number of clusters.
- Compare K-Means with Ward-linkage Agglomerative Clustering.
- Use PCA to visualize clusters and test clustering after reducing dimensionality.
- Interpret cluster composition using diagnosis labels only after clustering.
Supervised evaluation
- Use a stratified train/test split.
- Evaluate Logistic Regression with scaling fitted on training data only.
- Use 5-fold cross-validation.
- Tune Random Forest hyperparameters with GridSearchCV.
- Compare accuracy, precision, recall, F1-score, ROC-AUC, and malignant recall.
Files
- week3_unsupervised.ipynb — notebook with code, outputs, plots, and analysis prompts.
- requirements.txt — required Python packages.
- README.md — project overview and setup instructions.
- Week3_Report.docx — written report based on the notebook's actual results.
Setup
Python 3.10 or newer is recommended.

Create a virtual environment:
python -m venv .venv
Activate it on Windows:
.venv\Scripts\activate
Activate it on macOS/Linux:
source .venv/bin/activate
Install dependencies:
pip install -r requirements.txt
Launch Jupyter:
jupyter notebook

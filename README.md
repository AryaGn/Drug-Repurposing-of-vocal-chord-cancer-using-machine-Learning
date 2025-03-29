# Drug-Repurposing-of-vocal-chord-cancer-using-machine-Learning
This script loads datasets, preprocesses the data, and applies machine learning to classify whether a drug is effective (1) or ineffective (0) based on drug properties and gene expression data.

three datasets:

DrugBank_Drugs_All.csv: Contains drug-related features.

gene_expression.csv: Contains gene expression profiles.

labels.csv: Contains the ground-truth effectiveness of drugs.

Merges drug data, gene expression data, and labels using DrugID.

Data Cleaning & Preprocessing

Selects only numeric features.

Handles missing values by replacing them with the mean.

Standardizes features using StandardScaler.

 Dimensionality Reduction using PCA

Reduces high-dimensional data to at most 50 principal components.

 Train a Machine Learning Model

Splits the data into training (80%) and testing (20%) sets.

Uses a Random Forest Classifier to train on the drug-gene feature set.

 Evaluate the Model

Predicts the drug effectiveness on test data.

Computes accuracy, classification report, and ROC-AUC Score (if applicable).

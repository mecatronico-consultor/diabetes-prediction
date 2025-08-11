## Comparative Analysis of Classification Algorithms for Diabetes Prediction

# 📈 Overview
This repository contains a Jupyter notebook that performs a comprehensive and comparative analysis of 12 machine learning algorithms for a binary classification problem: predicting the onset of diabetes.

The main objective of the project is to clean, preprocess, and model the Pima Indians Diabetes Dataset to determine which classification algorithm offers the highest prediction accuracy.


# 📋 Dataset
This project uses the Pima Indians Diabetes Dataset. This dataset contains several medical predictor variables and a target variable indicating whether a patient has diabetes (1) or not (0).


# The features include:

Pregnancies

Glucose

BloodPressure

SkinThickness

Insulin

BMI

DiabetesPedigreeFunction

Age


# ⚙️ Methodology
The workflow followed in the notebook is as follows:

Data Loading and Exploration: The diabetes.csv dataset is loaded, and an initial exploration is performed to understand its structure and data types.

Data Cleaning: Implausible zero values were identified in columns like Glucose, BloodPressure, BMI, etc. These values were treated as missing data, replaced with NaN, and then imputed with the mean of their respective columns.

Data Preparation:

The dataset was split into features (X) and the target variable (y).

The data was segmented into training (80%) and testing (20%) sets using stratified sampling to maintain class proportions.

The features were scaled using StandardScaler to normalize their ranges and improve model performance.

Model Training and Evaluation: A set of 12 classification models were trained and evaluated. For each model, the following metrics were calculated on the test set:

Accuracy

Classification Report (Precision, Recall, F1-score)

Confusion Matrix, visualized as a heatmap.


# 🤖 Models Evaluated
The following algorithms were implemented and compared:

Logistic Regression

K-Nearest Neighbors

Decision Tree

Gaussian NB (Naive Bayes)

Linear Discriminant Analysis (LDA)

Random Forest

Extra Trees

AdaBoost

Gradient Boosting

Bagging

Perceptron

Support Vector Classifier (SVC)


# 📊 Results
The comparative analysis showed that ensemble-based algorithms, such as Random Forest and Gradient Boosting, achieved the best performance for this problem. The Random Forest model achieved the highest accuracy with 77.9% on the test set.

The accuracy comparison table is shown below:

Algorithm	Accuracy
Random Forest	0.779221
Gradient Boost	0.766234
Extra Trees	0.753247
AdaBoost	0.746753
SVC	0.733766
K-Nearest Neighbors	0.733766
Bagging	0.720779
Logistic Regression	0.694805
LDA	0.694805
Gaussian NB	0.694805
Perceptron	0.694805
Decision Tree	0.668831


Matplotlib & Seaborn: For data visualization.

Jupyter Notebook: As the interactive development environment.

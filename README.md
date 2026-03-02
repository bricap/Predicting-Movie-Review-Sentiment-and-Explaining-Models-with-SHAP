# Predicting-Movie-Review-Sentiment-and-Explaining-Models-with-SHAP
## Explaining Models with SHAP

This project demonstrates how SHAP (SHapley Additive exPlanations) can be used to interpret and explain machine learning model predictions. Using a sentiment analysis task on the IMDB movie reviews dataset, the notebook shows how SHAP values attribute feature importance and explain individual predictions in a transparent, interpretable way.

The project is based on Scott Lundberg’s SHAP demo and focuses on explaining a logistic regression text classification model built with TF-IDF features.

Project Overview

Machine learning models are often treated as “black boxes,” making it difficult to understand why a model makes a particular prediction. SHAP addresses this by assigning each feature a contribution value based on game theory, allowing us to break down predictions into meaningful explanations.

In this project, we:

Train a sentiment analysis model on movie reviews

Evaluate model performance

Use SHAP to explain both global and individual predictions

Visualize feature importance and word-level contributions to sentiment

Dataset

IMDB Movie Reviews Dataset

Binary classification task: Positive vs. Negative sentiment

Text data is transformed using TF-IDF vectorization

Methodology

Data Loading & Preprocessing

Load IMDB reviews

Split into training and test sets

Convert text to numerical features using TF-IDF

Model Training

Train a Logistic Regression classifier

Evaluate accuracy on the test set

Model Explainability with SHAP

Initialize a LinearExplainer

Compute SHAP values for test data

Generate:

Summary plots

Dependence plots

Force plots for individual predictions

Analyze which words contribute most to positive and negative sentiment

Key Visualizations

SHAP Summary Plot
Shows the most influential words across all predictions

Dependence Plots
Illustrate how specific words (e.g., fun, awful) affect predictions

Force Plots
Break down individual reviews to show word-level contributions

Use Cases

Model explainability is critical in many real-world applications, including:

Finance: Explaining loan approval or rejection decisions

Healthcare: Understanding risk factors driving predictions

Ethical AI: Improving transparency, fairness, and trust in models

Files in This Repository

Explaining_models_with_SHAP_CapuanoBrianna.ipynb
Main notebook containing all analysis, visualizations, and explanations

Technologies Used

Python

scikit-learn

SHAP

NumPy

Pandas

Jupyter Notebook

Results

Achieved ~85% accuracy on the IMDB test set

Identified meaningful word-level contributions to sentiment predictions

Demonstrated how SHAP can make linear models more interpretable and transparent

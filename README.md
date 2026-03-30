End-to-End Machine Learning Pipeline for Life Cycle Assessment (LCA) Impact Prediction

This repository contains an end-to-end Machine Learning pipeline specifically designed to bridge the gap between Machine Learning (ML) and Life Cycle Assessment (LCA).

The goal is to automatically test, optimize, and evaluate various regression models to accurately predict environmental impacts. Since LCA studies inherently deal with multiple impact categories at once (e.g., climate change, acidification, freshwater ecotoxicity), this script is built to handle multiple target variables simultaneously, making it much easier to run robust analyses on complex inventory datasets.

1- What does this code do?

In short, the script takes your .csv dataset and does all the heavy lifting for you:

Trains 13 predictive models, ranging from basic linear regressions to advanced tree-based algorithms (XGBoost, CatBoost, Random Forest) and Neural Networks.
Optimizes hyperparameters automatically using the Optuna framework.
Performs robust validation using Stratified K-Fold (10 folds) with multiple repeats.
Calculates detailed metrics, including R² (train and test), MSE, and an overfitting index.
Generates automated plots, including performance comparisons, trade-off charts (Computational Time vs. R²), and—crucially for environmental studies—feature explainability using SHAP.
Exports ready-to-use data, generating CSV spreadsheets with metric summaries and individual row-by-row predictions for further analysis.

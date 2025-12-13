📌 Overview

This repository contains the implementation and analysis for a machine learning coursework project focused on cuffless blood pressure (BP) estimation using phonocardiogram (PCG) signals. The project evaluates multiple regression-based machine learning models with a strong emphasis on statistical modelling concepts, model tuning, and generalisation analysis.

The study uses a publicly available PCG–BP dataset and applies classical regression techniques commonly used in biomedical signal processing.

🎯 Problem Statement

Conventional cuff-based blood pressure measurement is uncomfortable and unsuitable for continuous monitoring. Recent research shows that physiological signals, such as PCG, can encode information relevant to blood pressure.

The objective of this project is to:

Estimate systolic blood pressure from PCG signals

Compare multiple regression models from a statistical perspective

Analyse model performance, bias–variance trade-offs, and overfitting behaviour

📊 Dataset

Type: Public PCG–Blood Pressure dataset

Signals: Segmented phonocardiogram (PCG) recordings

Labels: Systolic blood pressure (SBP)

Additional features: Demographic attributes (age, gender, height, weight, pulse)

Privacy: No personally identifiable information (PII)

Availability: Public research dataset used strictly for academic purposes

🛠 Methodology
Feature Extraction

Short-Time Fourier Transform (STFT) applied to PCG signals

Time–frequency spectral features extracted

Features combined with demographic variables

Regression Models Evaluated

The following regression approaches were implemented and tuned explicitly:

Ridge Regression

Lasso Regression

Support Vector Regression (RBF kernel)

Decision Tree Regression

Gaussian Process Regression (RBF + WhiteKernel)

Each model was configured with non-default hyperparameters, selected based on the dataset size, signal characteristics, and statistical considerations.

📈 Evaluation Strategy

Train–test split

Metrics:

Mean Squared Error (MSE)

R-squared (R²)

Learning curves generated for all models

Bias–variance behaviour analysed statistically

🧪 Key Results (Summary)

Linear models (Ridge, Lasso) showed higher bias and limited performance

Support Vector Regression achieved strong generalisation

Decision Tree Regression achieved very low error but showed overfitting

Gaussian Process Regression provided the best overall performance, combining low error with statistical robustness and uncertainty modelling

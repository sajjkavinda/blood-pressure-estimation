Overview

This project investigates cuffless blood pressure (BP) estimation using phonocardiogram (PCG) signals and classical machine learning regression techniques. Traditional cuff-based BP measurements are uncomfortable and unsuitable for continuous monitoring. This work explores how statistical regression models can estimate systolic blood pressure from heart sound signals and demographic features.

The study focuses on model comparison, statistical interpretation, and generalisation behaviour, rather than deep learning, in line with the learning outcomes of the module.

Dataset

A publicly available PCG–BP dataset is used, containing:

- Segmented PCG audio recordings
- Corresponding systolic and diastolic BP values
- Demographic features (age, gender, height, weight)
- The dataset does not contain personally identifiable information (PII) and is suitable for academic research.

Methodology
Signal Processing

- PCG signals are converted to time–frequency representations using the Short-Time Fourier Transform (STFT)
- Extracted spectral features are combined with demographic variables
- Features are standardised prior to model training

Regression Models

The following regression models are implemented and tuned:

- Ridge Regression
- Lasso Regression
- Support Vector Regression (RBF kernel)
- Decision Tree Regressor
- Gaussian Process Regression (RBF + WhiteKernel)

All models use explicitly tuned hyperparameters to reflect dataset characteristics and statistical assumptions rather than default settings.

Evaluation

Models are evaluated using:

- Mean Squared Error (MSE)
- R-squared (R²)
- Learning Curves to analyse bias–variance trade-offs and overfitting behaviour

Key Findings

- Linear models show high bias when applied to complex physiological signals
- Kernel-based and probabilistic models better capture nonlinear BP relationships
- Learning curves are essential for diagnosing overfitting in biomedical datasets
- Gaussian Process Regression provides both accuracy and statistical robustness

Technologies Used

- Python
- NumPy, Pandas
- SciPy
- scikit-learn
- Matplotlib

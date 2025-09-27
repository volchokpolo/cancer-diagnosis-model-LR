# Breast Cancer Diagnosis Prediction Model

## Overview
A logistic regression classifier for predicting breast cancer diagnosis (malignant vs. benign) based on cytological features from fine needle aspirate (FNA) samples.

## Dataset Description
**Wisconsin Breast Cancer Dataset**
- **Source**: UCI Machine Learning Repository
- **Data Type**: Quantitative measurements derived from digitized images of fine needle aspirate (FNA) samples
- **Sample Size**: 569 patient samples
- **Features**: 30 numerical features describing cell nuclei characteristics
- **Target**: Binary classification (Malignant/Benign)

### Feature Categories
The 30 features represent measurements of cell nuclei in three statistical measures (mean, standard error, worst/largest values):
- **Size**: radius, area, perimeter
- **Shape**: smoothness, compactness, concavity, concave points, symmetry
- **Texture**: texture, fractal dimension

## Model Details
- **Algorithm**: Logistic Regression
- **Performance**: 94% accuracy
- **Libraries**: pandas, scikit-learn, numpy, matplotlib
- **Preprocessing**: Data cleaning (removed null columns), label encoding (M/B → 1/0), 75/25 train-test split, standardization of 30 morphometric features

## Clinical Context
Fine needle aspiration (FNA) is a minimally invasive diagnostic procedure where a thin needle extracts cells from suspicious breast lumps. This model aims to assist pathologists in diagnosis by analyzing quantitative features of cell nuclei morphology.

## Limitations & Future Work
- Limited to Wisconsin dataset characteristics
- Simple logistic regression - could explore ensemble methods
- No external validation on independent datasets

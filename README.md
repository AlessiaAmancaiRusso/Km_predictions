# Michaelis Menten (Km) Predictions for Enzyme-Substrate Pairs of Wild-type Enzymes

Internship project at the Institute of Computational Cell Biology - Heinrich Heine University, Düsseldorf. 



This repository contains scripts and notebooks for predicting the Michaelis constant (Km) of enzyme-substrate pairs by combining enzyme sequence embeddings with substrate molecular embeddings.

## Requirements

- **Python version:** 3.8
- **Python packages:**
  - numpy==2.2.6
  - pandas==2.2.3
  - matplotlib==3.9.0
  - seaborn==0.13.2
  - scikit-learn==1.6.1
  - scipy==1.13.1
  - rdkit
  - bioservices
  - tensorflow
  - xgboost
- **Software:**
  - InterProScan (used for protein domain annotation, requires a Linux environment)

## Repository Structure & Usage

- **Initial Analysis**
  - `Initial analysis/preprocessing.ipynb`  
   Performs all data preprocessing steps
  - `Initial analysis/training.ipynb`  
   Trains and validates models
  - `Initial analysis/results.ipynb`  
    Visualizes results

- **Data Preprocessing**
  - `Scripts/preprocessing_BRENDA.ipynb`  
    Preprocesses BRENDA dataset using the best method identified
  - `Scripts/preprocessing_SABIORK.ipynb`  
    Preprocesses SABIO-RK dataset and integrates both datasets together

- **Additional Features**
  - `Scripts/additional_features.ipynb`  
    Adds extra molecular and enzyme descriptors to input features

- **Model Training and Evaluation**
  - `Scripts/training.ipynb`  
    Implements model training and validation
  - `Scripts/results_dataset_comparison.ipynb`  
    Compares model performance across datasets
  - `Scripts/results_feature_importance.ipynb`  
    Analyzes feature importance in models
  - `Scripts/results_additional_input_features.ipynb`  
    Evaluates the effect of additional input features on predictions

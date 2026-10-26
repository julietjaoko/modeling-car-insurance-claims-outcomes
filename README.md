# Modeling Car Insurance Claims Outcomes

## Project Overview

This project focuses on modeling car insurance claim outcomes using customer and policy data. The main objective is to identify the factors that influence whether a claim is filed, approved, denied, or associated with a certain cost level. This is generally a classification or risk-modeling problem, and the notebook workflow includes data preparation, feature analysis, model building, and evaluation.

The project supports risk assessment and pricing strategy insights by uncovering patterns in claim behavior and loss severity.

## Dataset Summary

### Data Source

The dataset typically contains variables such as:

- policyholder demographics
- vehicle type and age
- driving history
- claim frequency
- accident history
- coverage type
- geographic region
- claim amount or outcome label

### Data Preprocessing

The analysis usually includes:

- loading the insurance dataset into a pandas DataFrame
- identifying missing or inconsistent values
- converting categorical variables to numeric or encoded features
- removing irrelevant or duplicated fields
- splitting the data into training and test sets
- evaluating models using appropriate classification metrics

## Project Structure

```text
.
├── README.md
├── data/
│   └── insurance_data.csv
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_preprocessing.ipynb
│   └── 03_modeling.ipynb
├── models/
│   └── insurance_model.pkl
├── outputs/
│   ├── classification_report.txt
│   └── visualizations/
└── .ipynb_checkpoints/
```

## Environment & Dependencies

### Using pip

```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Using conda

```bash
conda create -n insurance-modeling python=3.10
conda activate insurance-modeling
conda install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Notebook Execution Guide

Run the notebooks in order:

1. `notebooks/01_eda.ipynb`  
   Explore policy and claim distributions and relationships between features.

2. `notebooks/02_preprocessing.ipynb`  
   Prepare clean feature sets for modeling.

3. `notebooks/03_modeling.ipynb`  
   Train and compare classifiers or risk models.

If the entire workflow is contained in one notebook, run all cells sequentially from top to bottom.

## Key Findings & Results

The project aims to identify the strongest drivers of claims outcomes, such as:

- age and gender-related risk patterns
- vehicle type and policy coverage impact
- accident and claim frequency relationships
- geographic or demographic drivers of loss risk

Depending on the task, the model may be evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- confusion matrix

The final insights help explain which factors are most associated with claims severity or claim probability, supporting better risk assessment and actuarial decision-making.

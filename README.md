# Sowing Success: Machine Learning for Crop Selection

## Overview

This project aims to assist farmers in selecting the best crop to plant based on soil conditions. By leveraging machine learning techniques, we predict the optimal crop type using soil metrics such as nitrogen, phosphorous, potassium levels, and pH values. The goal is to maximize crop yield while considering soil suitability and agricultural efficiency.

## Dataset

The dataset `soil_measures.csv` provided contains:
- `N`: Nitrogen content ratio in the soil
- `P`: Phosphorous content ratio in the soil
- `K`: Potassium content ratio in the soil
- `pH`: pH value of the soil
- `crop`: Categorical values representing various crop types (target variable)

Each row in the dataset represents soil measurements for a specific field, with the corresponding optimal crop specified in the `crop` column.

## Project Structure

- `soil_measures.csv`: Dataset containing soil metrics and optimal crop types.
- `crop_selection.ipynb`: Jupyter notebook containing the project code for data exploration, model training, and evaluation.
- `README.md`: This file providing an overview of the project.

## Methodology

### 1. Data Exploration and Preparation
- Load and inspect the dataset.
- Separate features (`N`, `P`, `K`, `pH`) from the target variable (`crop`).

### 2. Model Building
- Split the data into training and test sets.
- Build logistic regression models for each soil metric (`N`, `P`, `K`, `pH`) to predict crop types.
- Evaluate model performance using the F1-score metric.

### 3. Identifying the Best Predictive Feature
- Determine the most important soil metric for predicting crop types based on F1-score.

## Results

- The model identified `K` (Potassium content) as the most predictive feature for determining crop types, achieving an F1-score of 0.239.

## Usage

1. Clone the repository:
   ```sh
   git clone https://github.com/NonsoOmoko/Project-Predictive-Modeling-for-Agriculture.git
   cd Project-Predictive-Modeling-for-Agriculture

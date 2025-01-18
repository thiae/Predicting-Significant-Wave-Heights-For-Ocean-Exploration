# Predicting_Significant_Wave_Heights_For_Ocean_Exploration
This project involves building and evaluating predictive models for significant wave heights (Hsig) based on environmental and oceanic conditions
# 🌊 Predicting Significant Wave Heights for Ocean Exploration

## Project Overview
This repository contains my solution to an assessment project aimed at predicting **Significant Wave Heights (`Hsig`)** for the Global Ocean Exploration Initiative (GOEI). The questions have been removed for conciseness; only the implementation code is provided.

This project involves preprocessing, feature engineering, model selection, and evaluation to build a robust machine-learning pipeline for predicting wave heights based on environmental and oceanic data.

---

## 🧾 Problem Statement
The goal is to predict significant wave heights (`Hsig`) using features such as wind speed, wave direction, water depth, and seasonal variations. This prediction is crucial for ensuring safe and efficient marine operations.

### Dataset
The dataset includes the following columns:
- `Hsig`: Significant wave height (target variable).
- `Temperature`: Water temperature (continuous or categorized).
- `Wind Speed`: Speed of wind in m/s.
- `Wave Direction (Dir)`: Direction from which waves approach (0° - 360°).
- `Depth`: Water depth in meters.
- `X-Windv`, `Y-Windv`: Wind velocity components.
- `Season`: Categorical seasons (e.g., Winter, Summer).
- `Wind_Dir_Category`: Simplified wave direction (e.g., North, East).

---

## 📋 Project Objectives
1. **Data Preprocessing and Feature Engineering**:
   - Address data preparation tasks, such as splitting into train and test sets, handling missing values, and creating meaningful features.
   - Develop a preprocessing pipeline (`prep_pipe`) to standardize and simplify transformations.

2. **Model Selection and Evaluation**:
   - Establish a baseline model using a parametric linear regression.
   - Compare performance with ensemble models tuned using `RandomizedSearchCV`.
   - Evaluate all models on both training (cross-validation) and test sets using R² and MSE metrics.

---

## 🛠️ Methodology
1. **Exploratory Data Analysis (EDA)**:
   - Understand relationships between variables and potential data issues.

2. **Data Preprocessing**:
   - Clean and transform data using a pipeline (`prep_pipe`).

3. **Feature Engineering**:
   - Explore transformations (e.g., binning, interaction terms).

4. **Modeling**:
   - Baseline Model: Linear Regression.
   - Ensemble Models: Two ensemble methods tuned with `RandomizedSearchCV`.

5. **Evaluation**:
   - Use R² and MSE metrics to select the best model (`final_model`) and assess performance on the test set.

---

## 📝 Deliverables
1. **Code**:
   - All preprocessing, modelling, and evaluation steps are implemented in Python.
2. **Pipeline**:
   - A structured and reusable pipeline for data preprocessing and modelling.
3. **Documentation**:
   - Markdown summaries for all steps, explaining the rationale and approach.
4. **Final Model**:
   - A well-tuned model saved as `final_model`.
   - Documented best hyperparameters as `Best_parameters`.

---

## 🎯 Key Takeaways
This repository demonstrates the ability to:
- Process and engineer features from real-world environmental datasets.
- Build and evaluate robust machine learning models for regression problems.
- Communicate results and methodology effectively through clear documentation.

---

## 📂 Repository Structure
- `README.md`: Overview and project description (this file).
- `Hs.csv`: Dataset provided by GOEI for the project.
- `notebooks/`: Contains Jupyter notebooks for EDA, preprocessing, modelling, and evaluation.
- `models/`: Serialized versions of trained models (e.g., `final_model.pkl`).
- `results/`: Performance metrics and evaluation results (e.g., R² and MSE).

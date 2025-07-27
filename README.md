```markdown
# Air Pollution Deaths ML Project

This project analyzes air pollution-related deaths over time across different countries. It explores trends using linear regression and advanced machine learning models, combining multiple datasets to deepen insights into environmental and socio-economic factors influencing mortality.

## Project Overview

We start by examining a Kaggle dataset on deaths due to air pollution (1990–2017) across various countries. The data is visualized, and linear regression models are developed at both regional and national levels to predict trends in mortality over time. These models effectively capture linear trends and allow for future death predictions, though they have limitations in many countries where relationships may be nonlinear.

To enrich the analysis, we merge the air pollution dataset with socio-demographic and economic data from:

- **Global Burden of Disease Study 2019 Results** via OECD.stats  
- **World Bank Development Indicators**

This merged dataset is then explored using three tree-based machine learning models to understand complex interactions between features.

## Repository Structure

The folder `AirPollution_Scripts` contains segmented scripts/notebooks organized for clarity and convenience.

### Suggested order for running the notebooks:

1. **`MLProject_AirPollution_Viz_LR.ipynb`**  
   Loads the initial Kaggle air pollution deaths dataset, processes and visualizes it, performs linear regression analysis, and makes future death predictions.

2. **`MLProject_DataProcessing_OECD_WB_GBD.ipynb`**  
   Loads raw data from World Bank and GBD/OECD datasets, cleans, merges them, and experiments with fuzzy dataset merging techniques.

3. **`MLProject_Exploratory_ML_Models.ipynb`**  
   Loads the cleaned and merged dataset, applies KNN regressor and model selection using PyCaret, and discusses model insights.

4. **`MLProject_ML_Models_refined.ipynb`**  
   Develops selected machine learning models (Extra Trees, Random Forest, XGBoost), performs cross-validation and ensemble methods, and discusses results.

## Data Sources

- **Primary dataset:** [Air Pollution Deaths (Kaggle)](https://www.kaggle.com/datasets/akshat0giri/death-due-to-air-pollution-19902017?resource=download)  
- **Supplemental data:**  
  - [Global Burden of Disease Study 2019 Results (OECD.stats)](https://stats.oecd.org/index.aspx?lang=en#)  
  - [World Bank Development Indicators](https://databank.worldbank.org/source/world-development-indicators#)

## Project Goal

The project aims to explore, supplement, and model trends in deaths caused by environmental factors, ultimately enabling more informed predictions of future mortality risks related to air pollution worldwide.

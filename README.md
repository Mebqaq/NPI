# Code Repository for "A half-life inspired measure of nighttime activity decay across cities"

This repository contains the Jupyter Notebooks used to produce the analysis and figures presented in the manuscript.

## Data Requirements
All datasets required to run these scripts should be placed in the relative `data` directory (`./data/`) before executing the notebooks.

## Code Structure

The analysis is divided into four main parts, corresponding to the "Results" section of the paper:

* **`result1.ipynb`**: Evaluates the universal decay patterns of nighttime activity. Contains code for fitting the Weibull distribution and calculating the Night Pulse Index (NPI). *(Corresponds to Figure 2)*
* **`result2.ipynb`**: Analyzes the relationship between nighttime activity rhythm, intensity, and semantic content. Demonstrates the orthogonal nature of the NPI. *(Corresponds to Figures 3 & 4)*
* **`result3.ipynb`**: Maps the spatial distribution of NPI and analyzes temporal variations (seasonal and weekday/weekend), confirming the "south-late, north-early" pattern. *(Corresponds to Figure 5)*
* **`result41.ipynb`, `result42.ipynb`, `result43.ipynb`**: Conducts the exploratory analysis of the variables associated with the NPI. Includes the Spatial Error Model (SEM) baseline, XGBoost modeling with SHAP values for nonlinear associations, and the interpretable city typology clustering. *(Corresponds to Figures 6 & 7)*

## Dependencies
The code requires standard Python data science and geospatial libraries, including but not limited to:
`pandas`, `numpy`, `scikit-learn`, `xgboost`, `shap`, `geopandas`, and `statsmodels` (or `pysal` for spatial modeling).
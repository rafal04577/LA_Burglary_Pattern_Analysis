# LA Burglary Pattern Analysis

This project explores burglary trends in Los Angeles using public crime data from 2020 onwards. The goal is to identify spatial and temporal patterns in burglary incidents and develop models to predict arrest outcomes, supporting data-driven decisions in urban safety and policing.

---

## Objectives
- Analyse burglary incidents across time, location, and demographics  
- Train classification models to predict whether an incident results in an arrest  
- Use SHAP values to understand model behaviour and feature impact  

---

## Dataset
A filtered sample of 8,000 burglary-related crime records from the LAPD dataset (2020–present). The full dataset exceeds 200MB and is publicly available online.

"la_burglary_data_sample.csv" – sampled for GitHub size limit  
Full dataset (219MB): [LAPD Open Data Portal](https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8)

Key fields:
- Crime type, report and occurrence dates  
- Premise type, area code, and location  
- Victim demographics  
- Arrest made (yes/no)

---

## Tools & Technologies
- Python (pandas, scikit-learn, SHAP, matplotlib, seaborn)  
- Jupyter Notebook

---

## Features
- Classification models: Logistic Regression, Random Forest  
- Evaluation: ROC AUC, confusion matrix, classification report  
- Data cleaning: missing values, categorical filtering, outlier handling  
- Visualisations: time-series plots, area-level heatmaps, SHAP plots

---

## Results & Insights
- Burglary hotspots identified in specific LAPD divisions  
- Arrest likelihood correlated with location type, day of the week, and victim gender  
- SHAP analysis revealed feature impacts on prediction outcomes  

---

## Files Included
- `LA_Burglary_Pattern_Analysis.ipynb`: Cleaned and structured notebook  
- `la_burglary_data_sample.csv`: Sampled dataset used for analysis  
- `LICENSE`: MIT License  

---

## Future Enhancements
- Integrate additional years of data for trend robustness  
- Use geospatial clustering for hotspot detection  
- Train ensemble models for improved arrest prediction

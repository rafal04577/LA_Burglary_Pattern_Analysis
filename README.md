# LA Burglary Pattern Analysis

This project explores burglary trends in Los Angeles using public crime data from 2020 onwards. It applies exploratory data analysis, geospatial mapping, and predictive modelling to help understand factors influencing arrest outcomes in burglary incidents.

---

## Objectives
- Analyse burglary incidents across time, geography, and victim characteristics  
- Engineer features such as time-of-day and seasonality to enhance model inputs  
- Train classification models to predict whether an incident results in an arrest  
- Use SHAP values to understand model decisions and identify influential predictors  

---

## Dataset
Sampled and cleaned burglary records from the LAPD open data portal (2020–present). Original dataset size exceeded 200MB.

"la_burglary_data_sample.csv" - sampled data included for reproducibility  
Full source: [LAPD Crime Data](https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8)

Key fields used:
- Report date, time, area, crime description, premise type, victim age/gender  
- Location coordinates, arrest indicator

---

## Tools & Technologies
- Python (pandas, scikit-learn, SHAP, matplotlib, seaborn, folium, plotly)  
- Jupyter Notebook

---

## Features
- Data preprocessing: handling nulls, removing duplicates, grouping and filtering burglary cases  
- Feature engineering: time-based segments (e.g. hour, weekday, season), victim attributes  
- Visualisation:
  - Static: heatmaps, bar plots, and time series charts  
  - Interactive: folium and plotly-based maps showing burglary density and district patterns  
- Classification models: Logistic Regression, Random Forest  
- Evaluation metrics: ROC AUC, confusion matrix, classification report  
- SHAP analysis: feature contribution visualisation for model interpretability  

---

## Results & Insights
- Certain districts showed persistently high burglary rates (e.g. Central, Hollywood)  
- Arrest likelihood varied with location type and temporal factors  
- SHAP values highlighted the predictive value of location, victim demographics, and time features  

---

## Files Included
- `LA_Burglary_Pattern_Analysis.ipynb` - cleaned and annotated notebook  
- `la_burglary_data_sample.csv` - representative subset of the full dataset  
- `LICENSE` - MIT License

---

## Future Enhancements
- Integrate multi-year datasets for trend validation  
- Apply clustering techniques for hotspot detection  
- Test ensemble methods or temporal models for improved prediction

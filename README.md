# Property Fraud Identification
An unsupervised machine learning model in Python

## Description
- This is a group project from the *Fraud Analytics* course at Rady School of Management, UC San Diego.
- The goal was to identify property tax fraud by detecting unusual records using machine learning.
- Two unsupervised machine learning model were built to estimate the anomaly score of each record, and a final anomaly score was created to rank the suspicious records.

## Dataset
- New York City government open-source data.
- Included over 1 million real-world property records in New York City in 2010.

## Methods
- Performed exploratory data analysis, then conducted a data quality report.
- Cleaned data, removed invalid records, and filled in missing values for chosen fields.
- Created 3 value metrics including value per ft2 for lot area, value per ft2 for building area, and value per ft2 for building volume, and then created 9 new expert variables based on these metrics to help detecting unusual valuations.
- Reduced dimensionality using Principal Component Analysis (PCA). 
- Built the first model that transformed the Z-scaled principal component into an anomaly score.
- Built the second model that used Keras library to calculate the autoencoder error and the second anomaly score.
- Combine the results of the two models into a final anomaly score which then be used to rank all the tax records based on their likelihood of being fraudulent. 
- Reviewed 10 of the records with high anomaly scores to verify the results.

## Conclusion
- The fraud algorithms used worked well in identifying anomalous properties, but further investigation is needed to confirm whether the unusual records are cases of fraud. 
- Many analysts tend to become infatuated with the most advanced tools and algorithms, but we spent more time on designing the solution.

**Please refer to the report and code files for more detail**


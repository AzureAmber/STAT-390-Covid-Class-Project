# STAT-390-Covid-Class-Project
The data science capstone project from STAT 390 using a Covid dataset

It should be noted that this Github repository is a copy with slight adjustments of the actual repository in order to keep the contents simplified and easier to understand.
The contributors consists of **Cindy H., Willie X., and Erica Z.**

Simply refer to the `Final Report` word document to view the results of this class project.

**Purpose:** 
The purpose of this project was to find a time series COVID-19 dataset and apply the skills we've developed in the R sequence, as well as new time-series methodologies, to investigate a research question. As the dataset we acquired from Kaggle spanned multiple countries and was updated regularly, we decided upon the following research task: To predict new cases of COVID-19 for G20 and G24 countries on the COUNTRY level. 

**Methodologies:**
Below is a quick outline of the methods we've applied throughout this project. 
- Checking time-series applicability using ADF test of stationarity
- Apply K-Means clustering to impute missingness
- Apply Cook's distance to determine outliers
- Building regressive models (ARIMA, Auto ARIMA, Prophet Univariate & Multivariate, XGBoost, Keras LSTM) with RMSE as performance metric
    - Tuning hyperparameters for these models with rolling origin validation sets and regular grids

**Instructions to Run Code:**
We have keep this repository neat and intuitive to the best of our capabilities over a 3 month time-span
- `data`: This folder contains our raw data, processed data (after intial data cleaning), and finalized data (training and testing for linear, tree-based, & neural network). 
- `Preprocessing Code`: This folder our EDA and data preprocessing steps. 
- `Reports`: This folder contains our weekly reports, proposal, and midterm report.
- `Models`: This folder contains all the R scripts for each models.
- `Results`: This folder contains all the visualizations for each model. This may include hyperparameter plots or Actual vs. Predicted New Cases per Country plots. 

To run any of the R scripts or code, please make sure that the dataset has been loaded into the RStudio environment. We have also made sure to include these lines of code at the top.
Additionally, some code may take more time to run (e.g. tuning), so we recommend looking at the commented out results or running the R script as a background job. 


**Dataset Source:** 
Our World in Data. (2023). Our World in Data - COVID-19 [Data set]. Kaggle. https://doi.org/10.34740/KAGGLE/DSV/6559049

Best, 
*Group 2: Cindy H., Willie X., Erica Z.*

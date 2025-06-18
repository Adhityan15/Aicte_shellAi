# Aicte_shellAi
Water Quality Prediction Using Machine Learning

Week 1 Summary: Data Collection & Preprocessing
Imported Required Libraries:
Used pandas, numpy, scikit-learn modules for data processing and model building.
Loaded the Dataset:
Loaded datasetwaterquality.csv using pandas.read_csv() with sep=';'.
Initial Data Exploration:
Inspected dataset structure with df.info(), df.describe(), df.shape, and checked for null values using df.isnull().sum().
Handled Date Column:
Converted date column from string to datetime format using pd.to_datetime().
Cleaned and Organized Data:
Sorted the dataset by id and date to maintain chronological order per location/station.
pollutants:
Selected target pollutants for modeling: ['O2', 'NO3', 'NO2', 'SO4', 'PO4', 'CL'].

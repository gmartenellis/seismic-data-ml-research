# Data

## Source

The primary dataset used in this project is the **Earthquakes in Japan** dataset available through Kaggle.

**Dataset:** Earthquakes in Japan
**Source:** Kaggle
**Coverage:** 2001–2018

The dataset contains recorded earthquake events and associated seismic characteristics used for data cleaning, exploratory analysis, feature preparation, dimensionality reduction, and clustering.

## Data Availability

The original dataset is not included in this repository.

To reproduce the analysis, obtain the dataset from its original Kaggle source and place the downloaded data file in this directory.

The notebooks contain the data-loading and preprocessing steps required for the analysis.

## Data Processing

The raw dataset is processed through the data-cleaning and exploratory-analysis workflow documented in:

`notebooks/01_eda_data_cleaning.ipynb`

The resulting prepared data is then used by:

`notebooks/02_ml_model.ipynb`

# Data

## Source

The dataset used in this project was obtained directly from the **U.S. Geological Survey (USGS) Earthquake Catalog**.

**Source:** USGS Earthquake Catalog
**Geographic scope:** Japan
**Coverage:** January 1, 2000 – August 2026

The data were retrieved using the USGS earthquake search interface with a geographic bounding box covering Japan and the specified date range.

## Dataset

After data cleaning and preparation, the final dataset contains:

* **16,815 earthquake records**
* **22 columns**
* **4 machine learning features**

The four features used for the machine learning analysis are:

* Longitude
* Latitude
* Magnitude
* Depth

The dataset contains additional earthquake catalog attributes that were retained during the data-preparation process but were not used as primary features in the clustering analysis.

## Data Availability

The downloaded USGS dataset is **not included in this repository**.

Because the data were obtained from the USGS Earthquake Catalog, users wishing to reproduce the analysis should retrieve the corresponding earthquake catalog data directly from the USGS using the documented geographic and temporal scope.

The repository does not redistribute the downloaded earthquake data.

## Data Processing

The dataset is processed through the data-cleaning and exploratory-analysis workflow documented in:

`notebooks/01_EDA_Data_Cleaning.ipynb`

The prepared data are then used for dimensionality reduction and unsupervised machine learning in:

`notebooks/02_ML_Modeling.ipynb`

The machine learning workflow uses the four selected features—longitude, latitude, mag

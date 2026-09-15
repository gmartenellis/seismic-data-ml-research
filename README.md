# Seismic Data ML Research

## Overview

This repository contains the code, analysis, and results for a graduate-level computer science capstone project focused on applying machine learning and data analysis techniques to earthquake data.

The project examines seismic activity in Japan using a historical earthquake catalog and explores whether computational methods can identify meaningful **spatial, temporal, and feature-based patterns** within the data.

Rather than attempting to predict individual earthquakes, the project focuses on using data-driven methods to **characterize and analyze patterns in observed seismic activity**.

---

## Project Objectives

The project was developed to:

* Prepare and validate a real-world seismic dataset for machine learning analysis.
* Explore spatial, temporal, and statistical characteristics of earthquake activity.
* Identify relationships and patterns among selected seismic features.
* Apply dimensionality-reduction and clustering techniques to the prepared data.
* Evaluate the usefulness of unsupervised machine learning for exploring seismic patterns.
* Demonstrate a reproducible machine learning workflow using Python.

---

## Dataset

The analysis uses the **Earthquakes in Japan** dataset covering earthquake events from **2001–2018**.

The dataset contains seismic event information that can be used to examine characteristics such as:

* Magnitude
* Depth
* Latitude
* Longitude
* Date and time
* Other recorded earthquake attributes

The dataset was obtained from Kaggle and is not redistributed through this repository.

---

## Methodology

The project follows a structured data analysis and machine learning workflow.

### 1. Data Preparation

The raw earthquake data was examined and prepared for analysis through:

* Data inspection
* Data-type validation
* Missing-value assessment
* Duplicate assessment
* Feature selection
* Data cleaning and transformation

### 2. Exploratory Data Analysis

Exploratory analysis was conducted to understand the characteristics of the seismic catalog and identify relationships among the selected variables.

The analysis examines patterns related to:

* Earthquake magnitude
* Earthquake depth
* Geographic location
* Temporal activity
* Relationships among seismic features

Visualizations are used throughout the analysis to support interpretation of the data.

### 3. Dimensionality Reduction

**Principal Component Analysis (PCA)** is used to transform the selected seismic features into a lower-dimensional representation.

This provides a way to examine the underlying structure of the feature space while reducing redundancy among correlated variables.

### 4. Clustering

Unsupervised clustering is used to investigate whether earthquake events form meaningful groups based on their characteristics.

The clustering analysis provides a computational approach for exploring patterns within the seismic catalog without relying on predefined class labels.

### 5. Evaluation and Interpretation

The resulting patterns are examined using appropriate quantitative measures and visualizations.

The analysis focuses on understanding:

* The characteristics of identified clusters
* Relationships among seismic features
* Spatial and temporal distribution of observations
* The usefulness and limitations of the applied machine learning techniques

---

## Project Structure

```text
seismic-data-ml-research/
│
├── README.md
│
├── notebooks/
│   ├── 01_eda_data_cleaning.ipynb
│   └── 02_ml_model.ipynb
│
├── data/
│   └── README.md
│
├── results/
│   └── figures/
│
├── src/
│
├── requirements.txt
│
└── .gitignore
```

The repository structure may evolve as the project is refined and additional documentation and results are added.

---

## Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**

---

## Key Areas of Analysis

The project combines several areas of computer science and data analysis:

**Data Engineering**

* Data ingestion
* Data cleaning
* Feature preparation

**Data Analysis**

* Exploratory data analysis
* Statistical examination
* Spatial and temporal analysis

**Machine Learning**

* Dimensionality reduction
* Unsupervised learning
* Clustering
* Model evaluation

**Data Visualization**

* Statistical visualizations
* Geographic analysis
* Cluster visualization
* Interpretation of multidimensional data

---

## Results

The analysis demonstrates how machine learning and visualization techniques can be applied to a seismic event catalog to explore relationships and patterns that may not be immediately apparent from the raw data.

Detailed results, visualizations, and interpretation are available in the project notebooks.

> **Note:** This project is an exploratory analysis of historical earthquake data. The results should not be interpreted as an earthquake prediction system or as evidence of causal relationships between seismic events.

---

## Limitations

Several limitations should be considered when interpreting the results:

* The analysis is based on a historical earthquake catalog and therefore reflects the characteristics and limitations of the available data.
* Clustering results depend on the selected features, preprocessing decisions, and machine learning parameters.
* Unsupervised clusters do not necessarily represent distinct physical or geological earthquake processes.
* The analysis identifies patterns in observed data but does not establish causation.
* The project does not provide operational earthquake forecasting or prediction.

---

## Future Work

Future development could extend the project through:

* Incorporating more recent seismic observations.
* Evaluating additional clustering approaches.
* Exploring additional feature-engineering strategies.
* Investigating alternative dimensionality-reduction techniques.
* Comparing results across different parameter configurations.
* Expanding visualization and interactive analytical capabilities.
* Developing a more comprehensive data pipeline for continued seismic-data analysis.

---

## Academic Context

This project was developed as a graduate capstone project for the **Master of Science in Computer Science** program at City University of Seattle.

The project demonstrates the application of computer science concepts—including data preparation, exploratory analysis, machine learning, dimensionality reduction, clustering, and visualization—to a real-world seismic dataset.

---

## Author

**Geraldine I. Marten-Ellis**

Graduate Student — Master of Science in Computer Science
City University of Seattle

# Seismic Data ML Research

## Overview

This repository contains the code, analysis, and results for a graduate-level computer science capstone project applying machine learning and data analysis techniques to a historical earthquake catalog.

The project uses earthquake data from Japan to explore **spatial, temporal, and feature-level patterns** in observed seismic events. The analysis focuses on how computational methods can be used to organize, transform, and examine multidimensional seismic data.

Rather than attempting to predict future earthquakes, this project uses **unsupervised machine learning** to explore patterns within an existing seismic event catalog.

---

## Project Objectives

The project was developed to:

* Prepare and validate a real-world seismic dataset for machine learning analysis.
* Explore the characteristics and relationships of selected earthquake features.
* Prepare seismic features for machine learning through data cleaning and transformation.
* Apply **Principal Component Analysis (PCA)** for dimensionality reduction.
* Apply **K-Means and DBSCAN** clustering to the prepared data.
* Compare and interpret the patterns produced by different unsupervised learning approaches.
* Demonstrate a reproducible Python-based machine learning workflow using real-world data.

---

## Dataset

The analysis uses the **Earthquakes in Japan** dataset covering earthquake events from **2001–2018**.

The dataset contains recorded earthquake information including variables such as:

* Magnitude
* Depth
* Latitude
* Longitude
* Date and time
* Other recorded seismic attributes

The original dataset was obtained from Kaggle and is **not redistributed in this repository**.

Instructions for obtaining and preparing the dataset are documented in [`data/README.md`](data/README.md).

---

## Methodology

The project follows a structured data analysis and unsupervised machine learning workflow.

### 1. Data Preparation

The earthquake catalog is examined and prepared for analysis through processes including:

* Data inspection
* Data-type validation
* Missing-value assessment
* Duplicate assessment
* Feature selection
* Data cleaning and transformation

The goal is to produce a consistent dataset suitable for subsequent exploratory analysis and machine learning.

### 2. Exploratory Data Analysis

Exploratory data analysis is used to examine the characteristics and relationships of the selected seismic variables.

The analysis considers dimensions such as:

* Earthquake magnitude
* Earthquake depth
* Geographic coordinates
* Temporal characteristics
* Relationships among selected features

The exploratory analysis provides context for the subsequent machine learning steps.

### 3. Principal Component Analysis

**Principal Component Analysis (PCA)** is applied as a dimensionality-reduction technique.

PCA transforms the selected features into principal components that represent the major sources of variation within the feature space. The resulting representation is then used to support visualization and clustering analysis.

### 4. Unsupervised Clustering

Two unsupervised machine learning approaches are applied:

* **K-Means clustering**
* **DBSCAN clustering**

K-Means partitions observations into a predefined number of clusters based on feature similarity, while DBSCAN identifies groups based on the density of observations and can distinguish observations that do not belong to dense clusters.

The two approaches provide complementary ways of examining structure within the seismic dataset.

### 5. Pattern Interpretation

The resulting clustering structures are examined through quantitative outputs and visualizations.

The analysis focuses on:

* Characteristics of the resulting clusters
* Relationships among the selected seismic features
* Differences between K-Means and DBSCAN results
* Patterns visible after dimensionality reduction
* Limitations associated with interpreting unsupervised clusters

The purpose is to evaluate the usefulness of these computational techniques for **exploratory analysis of seismic data**, rather than to establish physical causation or develop an operational forecasting system.

---

## Project Structure

```text
seismic-data-ml-research/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   ├── 01_EDA_Data_Cleaning.ipynb
│   ├── 02_ML_Modeling.ipynb
│   └── README.md
│
├── data/
│   └── README.md
│
├── results/
│   ├── README.md
│   └── figures/
│       ├── pca_kmeans.png
│       └── pca_dbscan.png
│
└── src/
    └── README.md
```

The repository structure is designed to separate analysis notebooks, data documentation, generated results, and reusable source code.

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

The project demonstrates several areas of computer science and data analysis.

### Data Preparation

* Data ingestion
* Data validation
* Data cleaning
* Feature selection
* Feature preparation

### Exploratory Data Analysis

* Descriptive analysis
* Feature relationships
* Spatial characteristics
* Temporal characteristics
* Multidimensional data exploration

### Machine Learning

* Principal Component Analysis
* Dimensionality reduction
* K-Means clustering
* DBSCAN clustering
* Unsupervised pattern analysis

### Data Visualization

* Exploratory visualizations
* PCA-based visualization
* Cluster visualization
* Comparative interpretation of machine learning results

---

## Results

The analysis demonstrates how dimensionality reduction and unsupervised clustering can be applied to a historical earthquake catalog to explore structure within multidimensional seismic data.

### PCA + K-Means

The PCA-reduced feature space was used to visualize the K-Means clustering results.

![PCA and K-Means clustering](results/figures/pca_kmeans.png)

### PCA + DBSCAN

The PCA-reduced feature space was also used to visualize the DBSCAN clustering results.

![PCA and DBSCAN clustering](results/figures/pca_dbscan.png)

These visualizations provide a direct comparison of the patterns identified by the two unsupervised clustering approaches.

---

## Limitations

Several limitations should be considered when interpreting the results:

* The analysis is based on a historical earthquake catalog and therefore reflects the characteristics and limitations of the available data.
* Results depend on the selected features and preprocessing decisions.
* Clustering results are sensitive to algorithm-specific parameters.
* Unsupervised clusters do not necessarily correspond to distinct physical or geological earthquake processes.
* The analysis identifies patterns in observed data but does not establish causal relationships.
* The project does not provide earthquake prediction or operational earthquake forecasting.

---

## Future Work

Potential extensions of the project include:

* Incorporating more recent seismic observations.
* Exploring additional feature-engineering strategies.
* Evaluating additional clustering algorithms.
* Investigating alternative dimensionality-reduction techniques.
* Comparing clustering results across different parameter configurations.
* Expanding visualization and analytical capabilities.
* Developing a more comprehensive and repeatable seismic-data processing pipeline.

---

## Academic Context

This project was developed as a graduate capstone project for the **Master of Science in Computer Science** program at City University of Seattle.

The project demonstrates the application of computer science concepts—including data preparation, exploratory data analysis, dimensionality reduction, unsupervised machine learning, clustering, and visualization—to a real-world seismic dataset.

---
## References

## Selected References

* Aiken, C., & Obara, K. (2021). Data-driven clustering reveals more than 900 small magnitude slow earthquakes and their characteristics. *Geophysical Research Letters, 48*(11). https://doi.org/10.1029/2020GL091764

* Beroza, G. C., Segou, M., & Mostafa Mousavi, S. (2021). Machine learning and earthquake forecasting—Next steps. *Nature Communications, 12*(1). https://doi.org/10.1038/s41467-021-24952-6

* Essing, D., & Poli, P. (2024). Unraveling earthquake clusters composing the 2014 Alto Tiberina earthquake swarm via unsupervised learning. *Journal of Geophysical Research: Solid Earth, 129*(1). https://doi.org/10.1029/2022JB026237

* Iaccarino, A. G., & Picozzi, M. (2023). Detecting the preparatory phase of induced earthquakes at the Geysers (California) using K-means clustering. *Journal of Geophysical Research: Solid Earth, 128*(10). https://doi.org/10.1029/2023JB026429

* Mousavi, S. M., & Beroza, G. C. (2023). Machine learning in earthquake seismology. *Annual Review of Earth and Planetary Sciences, 51*(1), 105–129. https://doi.org/10.1146/annurev-earth-071822-100323

* Piegari, E., Camanni, G., Mercurio, M., & Marzocchi, W. (2024). Illuminating the hierarchical segmentation of faults through an unsupervised learning approach applied to clouds of earthquake hypocenters. *Earth and Space Science, 11*(10). https://doi.org/10.1029/2023EA003267

* Zacchei, E., & Brasil, R. (2024). K-means for earthquakes: Disaggregation analyses of small events by considering wave components and soil types. *Arabian Journal of Geosciences, 17*(11). https://doi.org/10.1007/s12517-024-12113-0

* Kaggle. (n.d.). *Earthquakes in Japan (2001–2018)*. Dataset by aerodinamicc. The dataset was originally acquired from the USGS Earthquake Catalog.

The complete bibliography is maintained separately as part of the academic capstone documentation.

---
## Author

**Geraldine I. Marten-Ellis**

Graduate Student — Master of Science in Computer Science
City University of Seattle

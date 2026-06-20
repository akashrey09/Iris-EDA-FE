# Iris Data Analysis Report

## Project Overview

This project presents a comprehensive Exploratory Data Analysis (EDA) and Feature Engineering workflow using the Iris Dataset. The analysis focuses on understanding feature distributions, identifying relationships between variables, engineering meaningful features, and extracting actionable insights that can support machine learning model development.

The project has been transformed from traditional notebook-based analysis into an interactive web report, providing a structured and visually engaging way to explore the dataset.

## Live Demo

https://iris-data-report.lovable.app

---

## Dataset Information

The Iris Dataset contains 150 observations of iris flowers across three species:

* Iris Setosa
* Iris Versicolor
* Iris Virginica

### Features

| Feature      | Description                      |
| ------------ | -------------------------------- |
| Sepal Length | Length of the sepal (cm)         |
| Sepal Width  | Width of the sepal (cm)          |
| Petal Length | Length of the petal (cm)         |
| Petal Width  | Width of the petal (cm)          |
| Species      | Flower species (Target Variable) |

---

## Project Objectives

* Perform comprehensive Exploratory Data Analysis
* Assess data quality and completeness
* Analyze feature distributions and relationships
* Identify patterns across species
* Engineer meaningful features from existing variables
* Apply feature scaling techniques
* Perform feature selection
* Generate interpretable insights from the dataset

---

## Exploratory Data Analysis

### Data Quality Assessment

* Missing value analysis
* Duplicate record verification
* Data type validation
* Dataset structure inspection

### Statistical Analysis

* Descriptive statistics
* Variability analysis
* Skewness analysis
* Species-wise comparisons

### Visualization Techniques

* Histograms
* Boxplots
* Correlation heatmaps
* Pairplots
* Class distribution visualizations

### Correlation Analysis

* Feature-to-feature correlation analysis
* Feature-to-target relationship analysis
* Identification of highly predictive variables

---

## Feature Engineering

To improve feature representation and explore additional relationships, the following features were created:

### Petal Area

```python
PetalArea = PetalLength * PetalWidth
```

### Sepal Area

```python
SepalArea = SepalLength * SepalWidth
```

### Petal-Sepal Ratio

```python
PetalSepalRatio = PetalArea / SepalArea
```

These engineered features capture interactions between original variables and provide additional information for downstream machine learning tasks.

---

## Feature Scaling

Numerical features were standardized using StandardScaler to ensure consistent feature magnitudes and prepare the dataset for machine learning algorithms.

Key outcomes:

* Mean centered around 0
* Standard deviation scaled to 1
* Improved compatibility with distance-based algorithms

---

## Feature Selection

Forward Selection using Adjusted R² was implemented to identify the most informative features and reduce redundancy.

Key observations:

* Petal-related features consistently demonstrated higher predictive value.
* Sepal Width contributed less information relative to other variables.
* Feature selection confirmed the importance of petal measurements for species classification.

---

## Key Findings

* The dataset contains no missing values and no duplicate records.
* The target variable is perfectly balanced across all three species.
* Petal Length and Petal Width are the strongest predictors of flower species.
* Setosa forms a clearly separable cluster from the other species.
* Most classification complexity exists between Versicolor and Virginica.
* Strong positive correlation exists between Petal Length and Petal Width.
* Engineered features such as Petal Area and Petal-Sepal Ratio enhance feature representation and interpretability.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Statsmodels
* Lovable

---

## Project Structure

```text
├── iris_EDA.ipynb
├── iris_FE.ipynb
├── Iris_EDA_FE_Insights.txt
├── README.md
```

---

## Learning Outcomes

This project strengthened practical knowledge in:

* Data Cleaning and Validation
* Exploratory Data Analysis
* Statistical Interpretation
* Data Visualization
* Feature Engineering
* Feature Selection
* Data Preparation for Machine Learning
* Insight Communication

---

## Future Enhancements

* Implement machine learning classification models
* Compare multiple algorithms and evaluation metrics
* Add model performance visualizations
* Introduce interactive filtering and exploration features
* Deploy a predictive classification system

---

## Author

**Shresth Prakash**

B.Tech in Artificial Intelligence & Machine Learning

Focused on Data Science, Machine Learning, and Applied AI Solutions.



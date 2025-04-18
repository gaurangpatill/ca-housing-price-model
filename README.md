# ca-housing-price-model
This project involves Exploratory Data Analysis (EDA), data cleaning, and training various machine learning models to predict housing prices in California.

---

## 1. EDA and Data Cleaning

Thorough exploratory data analysis and preprocessing steps were conducted:

- **Initial Exploration**:
  - Inspected data types, null values, and summary statistics using `.info()`, `.describe()`, and `.value_counts()`.
- **Visualizations**:
  - Histograms for feature distributions.
  - Scatter plots to visualize geographical housing patterns (`longitude` vs. `latitude`).
  - Analyzed correlation using heatmaps.
- **Feature Engineering**:
  - Created new features like:
    - `rooms_per_household`
    - `bedroom_per_room`
    - `population_per_household`
- **Missing Values**:
  - Handled with `SimpleImputer` using median strategy.
- **Categorical Encoding**:
  - Transformed `ocean_proximity` using `OrdinalEncoder` and `OneHotEncoder`.
- **Data Splitting**:
  - Used `StratifiedShuffleSplit` for training/testing split based on income categories.

---

## 2. Training Machine Learning Algorithms

Trained and evaluated several models to predict `median_house_value`:

- **Linear Regression**:
  - Used as a baseline model.
- **Decision Tree Regressor**:
  - Captured non-linear relationships.
- **Random Forest Regressor**:
  - Improved performance with ensemble learning.
- **Evaluation**:
  - Metrics: Root Mean Squared Error (RMSE).
  - Applied cross-validation for robust performance estimates.
- **Pipeline**:
  - Combined all preprocessing steps into a pipeline for clean and efficient training.

---

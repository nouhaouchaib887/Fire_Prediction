# Wildfire Prediction Project

## Project Objective

This project aims to predict wildfire occurrences in two specific countries, Portugal and Greece. Using historical fire data, meteorological information, and vegetation data, we develop machine learning models to perform a binary classification task (fire/not fire).

---

## Data Sources

The data used in this project comes from multiple sources:

- **MODIS Data**: Historical fire data from satellites, covering Portugal and Greece for the year 2023.
- **Weather API**: Meteorological features extracted prior to fire events to enhance predictive accuracy.

---

## Notebook Structure

The project is organized into four main notebooks, each handling a specific phase of the process:

1. **Fire_Data**:
   - Loading and processing MODIS data for Portugal and Greece.
   - Generating "not fire" event data to introduce a binary classification task.

2. **Weather_Data**:
   - Extracting meteorological features using an API, focusing on conditions preceding fire incidents to enrich the predictive model.

3. **Vegetation_Data**:
   - Collecting and processing vegetation data from HDF files, leveraging geolocation techniques to pinpoint study areas.

4. **Modeling_Evaluation**:
   - Merging collected data, preprocessing, dimensionality reduction, and building various machine learning models.
   - Evaluating and comparing models using diverse performance metrics.

---

## Datasets

The project directory includes eight distinct datasets, each generated at specific stages of the project to be used in subsequent phases.

---

## How to Use

To execute this project:

1. Start with the `Fire_Data` notebook for initial data preparation.
2. Proceed with `Weather_Data` and `Vegetation_Data` for additional data collection.
3. Finally, use the `Modeling_Evaluation` notebook to build and evaluate predictive models.

Each notebook is self-contained and can be executed in a Jupyter environment with the necessary Python libraries installed, including scikit-learn, TensorFlow/Keras, Pandas, NumPy, and Seaborn/Matplotlib for visualization.

---

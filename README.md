# Sowing Success: Optimizing Crop Selection with Machine Learning

[![Crop Field](https://images.unsplash.com/photo-1527847263472-aa5338d178b8?q=80&w=2074&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)](https://unsplash.com/@jediahowen)

Photo by [Jed Owen](https://unsplash.com/@jediahowen) on [Unsplash](https://unsplash.com).

> *A machine learning solution for farmers to make data-driven decisions about crop selection.*

### Project Overview

Farmers face the challenge of selecting the best crop for their fields to maximize yield while managing costs. This project leverages machine learning techniques to help farmers identify the optimal crop based on essential soil metrics, including nitrogen, phosphorus, potassium, and pH levels. 

The project uses the **`soil_measures.csv`** dataset, which contains soil data for different fields and the corresponding optimal crop for each field.

### The Data

The dataset includes the following columns:

| Column  | Description                                                   |
|---------|---------------------------------------------------------------|
| `"N"`   | Nitrogen content ratio in the soil                            |
| `"P"`   | Phosphorous content ratio in the soil                         |
| `"K"`   | Potassium content ratio in the soil                           |
| `"pH"`  | pH value of the soil                                          |
| `"crop"`| The optimal crop for the field based on the soil composition (target variable) |

### Methodology

This project follows a structured approach to build a reliable classification model:

1. **Data Cleaning**:
  
   - Removed missing values accounting for less than 5% of the dataset to ensure data consistency.

2. **Data Preparation**:
  
   - Split the dataset into training and testing sets.
  
   - Built a **pipeline** to integrate data imputation, scaling, and model training into a single workflow.

3. **Feature Selection**:
  
   - Investigated each soil feature's predictive performance using accuracy as the metric.
  
   - Identified **potassium (K)** as the most predictive feature for determining the optimal crop.
  
      ![https://github.com/MohamedMostafa259/SowingSuccess_OptimizingCropSelectionWithMachineLearning/blob/main/AccuracyOfEachFeature.png](AccuracyOfEachFeature)

   - trained a model on all soil measurements in the dataset, and then investigated its accuracy for **optimizing crop selection** ($\approx$ 68%)

<br>

Don't hesitate to contribute to make a meaningful impact together :)

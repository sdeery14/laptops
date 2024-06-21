# Laptop Pricing Analysis

## Overview

This repository contains the final project for IST 707 - Applied Machine Learning, focusing on analyzing the Laptop League dataset from FlipKart. The project aims to explore the common configurations of laptops, identify their price points, and predict the price based on specific features.

## Report Contents

### 1. Introduction

- **Dataset**:
  - The dataset is sourced from FlipKart and contains detailed information on various laptop models, including specifications, ratings, and prices.
  - Key Variables: Company, Rating, Number of Ratings, Review, Size, Processor, RAM, Memory, Operating System, Price, and MRP (Manufacturer's Suggested Retail Price).

- **Project Goals**:
  - Determine common laptop configurations and their corresponding price points.
  - Predict the price of a laptop based on its specifications.

### 2. Data Preparation and Exploration

- **Data Cleaning**:
  - Removed irrelevant columns and corrected outlier values in the size and price fields.
  - Filled in missing or incorrect values for specific laptop configurations based on manual lookups.

- **Feature Engineering**:
  - Created new columns for processor manufacturer, disk size, and operating system from existing data.
  - Converted categorical variables to factors and normalized numerical values for model training.

- **Exploratory Data Analysis**:
  - Analyzed the distribution and relationships of key variables such as Company, Rating, Size, RAM, Disk Size, and Price.
  - Visualized data using ggplot2 to identify patterns and insights.

### 3. Statistical Modeling

- **Data Splitting**:
  - Split the data into training and testing sets to evaluate the performance of the models.

- **Models Used**:
  - **k-Nearest Neighbors (k-NN)**:
    - Predicted laptop price category based on closest data points in the training set.
  - **Support Vector Machine (SVM)**:
    - Used SVM to classify laptops into price categories based on their specifications.
  - **Random Forest**:
    - Employed random forest to predict laptop prices by averaging the results of multiple decision trees.
  - **Naive Bayes**:
    - Applied Naive Bayes classifier to model the probability of different price categories.
  - **Decision Tree**:
    - Built decision trees to model the decision process for categorizing laptop prices.

### 4. Key Insights and Findings

- **Common Configurations**:
  - Identified popular configurations based on size, RAM, and disk size across different brands and price points.
  - Analyzed the impact of these configurations on the overall price of laptops.

- **Price Prediction**:
  - Developed models to predict the price category of laptops based on their specifications.
  - Found significant predictors of price, including RAM size, disk size, and processor type.

- **Visualization and Analysis**:
  - Used ggplot2 to create comprehensive visualizations of the dataset, highlighting relationships between different variables and their influence on price.

### 5. Tools and Libraries

- **R Programming**:
  - Analysis and modeling were performed using R, with extensive use of libraries like ggplot2, dplyr, caret, and randomForest for data manipulation, visualization, and modeling.

## Authors

- Sean Deery
- Mark Stiles
- Chris Drabb


## How to Use This Repository

1. **Data Preparation**:
   - Run the `laptops-analysis.rmd` script to explore the data visualizations and ttrain the the machine learning models.
   - Ensure that the dataset `laptop_information.csv` is in the `data` folder.

3. **Review the Full Report**:
   - Access the `laptops-report.docx` file to read the detailed analysis and insights.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.




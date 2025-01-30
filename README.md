# Basic-EDA-in-python
## Overview
This project involves analyzing a housing dataset, performing data cleaning, feature engineering, and building a linear regression model to predict housing values. The dataset contains information about various housing features such as the number of rooms, bedrooms, population, and median income. The goal is to create insights into the relationship between these features and the median house value.

## Libraries Used
**pandas**: For data manipulation and analysis
**seaborn**: For creating attractive and informative statistical graphics
**matplotlib**: For data visualization
**sklearn**: For machine learning tasks such as linear regression and model evaluation

## Steps Taken

### 1. Data Loading
The dataset is loaded using pandas' read_csv function.

### 2. Data Cleaning
Dropped irrelevant columns such as longitude, latitude, total rooms, total bedrooms, population, and ocean proximity.
Removed missing values using the dropna() function.

### 3. Feature Engineering
Created new features like:
rooms_per_household: Total rooms divided by households
bedrooms_per_household: Total bedrooms divided by households
population_per_household: Total population divided by households

### 4. Data Transformation
Rounded the newly created features to 0.5 for rooms_per_household and bedrooms_per_household.
Rounded population_per_household to the nearest integer.

### 5. Data Visualization
A correlation matrix is plotted to visualize relationships between features, helping to identify any strong correlations.

### 6. Model Building
Split the dataset into training and testing sets.
Built a linear regression model to predict median_house_value based on other features.
Evaluated the model using the R-squared score, which measures the proportion of variance in the dependent variable (house values) explained by the model.

### 7. Results
The R-squared score of the model is approximately 0.532, indicating that the model can explain 53.2% of the variance in house prices based on the selected features.


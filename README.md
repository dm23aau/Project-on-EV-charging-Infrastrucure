# Project-on-EV-charging-Infrastrucure

## Project Overview
The goal of this project is to analyze and predict the behavior of EV charging stations using historical data. The key steps include:

   - Data Cleaning and Preprocessing.
   - Exploratory Data Analysis (EDA) to understand usage patterns.
   - Time Series Forecasting using ARIMA models.
   - Clustering analysis to identify patterns in station usage.
    -Predicting the availability of charging stations using machine learning models

## Dataset Description
The dataset used in this project (station_data_dataverse.csv) includes various features such as:

    -stationId: Unique identifier for each charging station.
    -created: Timestamp when a charging session started.
    -ended: Timestamp when a charging session ended.
    -kwhTotal: Total energy consumed during the session.
    -chargeTimeHrs: Duration of the charging session.
    -distance: Distance to the nearest charging station.
    -facilityType: Type of facility where the station is located

## Models Used
- ARIMA (AutoRegressive Integrated Moving Average):Used for predicting usage trends of electric vehicle charging stations based on historical hourly data
- K-Means Clustering: Uesd to identify distinct patterns in the charging station usage data, facilitating the categorization of charging stations based on usage patterns
- Random Forest: Used for its robustness and effectiveness in handling overfitting.
- Logistic Regression: Employed for its efficiency in binary classification tasks.
- Convolutional Neural Network (CNN): Utilized for capturing time-dependent patterns in station usage data.

## Installation
To run this project, you will need Python and several libraries installed. 

## Features and Labels
The key features include:
- `kwhTotal`: Total kilowatts consumed during a session.
- `chargeTimeHrs`: Duration of the charging session.
- `distance`: Distance travelled before charging.
- `facilityType`: Type of facility where the charging station is located.

## Data Preprocessing
-Missing Values: The dataset was cleaned by removing rows with missing values in critical columns, such as distance.
-Date Formatting: The created and ended timestamps were corrected for inconsistent year formatting and converted to proper datetime objects.
-Feature Scaling: Numerical features were standardized to ensure fair comparison during clustering and modeling.

## Exploratory Data Analysis (EDA)
-Distribution Plots: Histograms and boxplots were used to visualize the distribution and identify outliers in key features like kwhTotal, chargeTimeHrs, and distance.
-Correlation Analysis: A heatmap was generated to understand the relationships between numerical features.
-Time-Based Analysis: The dataset was analyzed on an hourly and weekly basis to identify trends in usage.

## Time Series Forecasting
ARIMA Model: An ARIMA model was used to forecast the number of charging sessions per hour. The model was trained on the historical hourly data, and future trends were predicted.

## Clustering Analysis
K-Means Clustering: Stations were clustered based on their usage patterns (kwhTotal, chargeTimeHrs, and distance). The Elbow method was used to determine the optimal number of clusters.

## Availability Prediction
-Feature Engineering: Availability data was created by resampling the sessions to hourly intervals and labeling hours as available or unavailable.
-Machine Learning Models: Convolutional Neural Networks (CNN), Random Forest, and Logistic Regression models were trained to predict station availability.

## Model Evaluation
-Accuracy: The performance of each model was evaluated using accuracy metrics.
-Training History: The training process of the CNN model was visualized through accuracy and loss plots over epochs.

## Results
-The ARIMA model was instrumental in forecasting the hourly usage patterns, providing insights into peak times and potential off-peak incentives. 
-The k-means clustering algorithm helped categorize charging stations based on user interaction patterns, which is essential for targeted improvements and resource allocation.
-The CNN model achieved good accuracy in predicting station availability, outperforming traditional models like Random Forest and Logistic Regression.

## Acknowledgments
- Thanks to my Supervisor who have invested time in improving this project.
- Special thanks to data providers Kaggle.

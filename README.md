# Project-on-EV-charging-Infrastrucure
# Charging Station Availability Prediction

## Project Overview
This project aims to predict the availability of electric vehicle charging stations using various machine learning models. It includes implementations of Random Forest, Logistic Regression, and a Convolutional Neural Network (CNN) to determine the most effective model for predicting charging station status based on historical usage data.

## Dataset Description
The dataset includes information from high-resolution electric vehicle charging sessions, featuring details such as start and end times, energy consumption, and station identifiers. This data is used to train models that can predict whether a charging station will be available at a given time.

## Models Used
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

The label or target variable is:
- `available`: Binary indicator (0 or 1) showing whether the charging station is available.

## Evaluation
Each model's performance is evaluated based on accuracy. The results are documented in the Jupyter notebooks included in the repository.

## Acknowledgments
- Thanks to my Supervisor who have invested time in improving this project.
- Special thanks to data providers Kaggle.

# Used-Car-Price-Prediction-Machine-Learning-Project-
This project focuses on building a machine learning model to predict the selling price of used cars based on various features such as age, mileage, fuel type, transmission, and ownership history.
The dataset contains real-world car listing data with significant missing values and inconsistencies, making this a strong end-to-end data cleaning and modeling project.
## Objective
Predict the AskPrice of used cars accurately
Handle messy real-world data (missing values, inconsistent formats)
Compare multiple machine learning models
Optimize the best-performing model

## Dataset Description
The dataset contains 24,575 records with the following key features:

Year – Manufacturing 

Age – Age of the car

kmDriven – Distance driven

Transmission – Manual / Automatic

Owner – Ownership type

FuelType – Petrol / Diesel / etc.

PostedDate – Listing date

Brand_Model – Combined car brand & model

AskPrice – Target variable

## dataset used 
<a href="https://github.com/zulusanele626-byte/Used-Car-Price-Prediction-Machine-Learning-Project-/blob/main/used_cars_dataset%20(1).csv">dataset</a>

## Data Preprocessing & Feature Engineering
## Data Cleaning

Handled missing values using:

Extraction from text (AdditionInfo)
Forward fill / backward fill
Median imputation
Removed duplicates (~9,699 rows)

## Feature Engineering
Extracted:

Year, Fuel Type, Brand, Transmission from text
Created new features:
Age = Current Year - Year
AccidentFree, SingleOwner, WellMaintained (binary flags)
DaysSincePosting
Combined Brand + Model → Brand_Model
## Encoding
One-hot encoding for:

Transmission
Owner
FuelType
Brand_Model (top frequent only)
## Scaling
Standardized numerical features:

Age
kmDriven
DaysSincePosting

## Models Used
Model 	RMSE  	R² Score

Linear  Regression	 1,370,889	0.245

Random  Forest	 792,988	0.747

Ridge	 1,370,888 	0.245

Lasso 	1,370,888 	0.245

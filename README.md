
# Module 3 Final Project

by Shenghao (Lavender) Zhang

## Introduction

Potable water resource is key life necessity. In Tanzania, many areas depends on water pumps for living support. It is very important to learn the functionality status of water pumps and what are potential factors that might this. 
<img src = 'https://github.com/lavsz/Mod3_Tanzania_Pump_Functionality_Prediction/blob/master/Digital_Arts/Water_pump_with_seat_and_easy_access_(Tanzania)_(5600883227).jpg' width="450" height="250">

This project intends to look at different physical, geographical, and social features related to the water pump. 


## Questions to Study

- Would water features affect the functionality of the pump?
- Would operation factors affect the functionality of the pump?
- Are there any geospatial distribution patterns?
- Are there any particular characteristics standing out that can affect the functional status of the pump?

## Models & Evaluation
A few different types of machine learning models were utilized to study the functional status of the water pumps, including:
- Random Forest Classifier
- K-Nearest Neighbours (KNN)
- XGBoost

Random Forest and XGBoost achieved the higher accuracy scores and were further tuned and evaluated. 

Final accuracy score for XGBoost: 79%

## Some Findings

Based on the EDA and model, some important feature include:
- Distance to the closest town
- Population (which infers further usage)
- Height (altitude)
- Total Static head
- Quantity
- Pemitting

## Resources
- Detailed Jupyter Notebook is [here](https://github.com/lavsz/Module3_Final_Project/blob/master/EDA_MODEL_master.ipynb)
- The Presentation slides is [here](https://github.com/lavsz/Module3_Final_Project/blob/master/Tanzania%20Water%20Pump.pdf)

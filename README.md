
# Module 3 Final Project

by Shenghao (Lavender) Zhang

## Introduction

Potable water resource is key life necessity. In Tanzania, many areas depends on water pumps for potable water access. It is very important to learn the functionality status of water pumps and what are potential factors that might this. This project intends to look at different physical, geographical, and social features in predicting whether water pumps are functional, needs repair, or non-functional. 

<img src = 'https://github.com/lavsz/Mod3_Tanzania_Pump_Functionality_Prediction/blob/master/Digital_Arts/Water_pump_with_seat_and_easy_access_(Tanzania)_(5600883227).jpg' width="200" height="150">

The original dataset is provided by Drivendata for competition. External sources were acquired to provide additional geospatial features, including: 
- Administrative Boundaries
- Towns
- Soil Type
- Landcover


## Key features to Visualize

Let's begin with looking at several different features in this dataset and see if they have any influences on functionality. 

**Would water features affect the functionality of the pump?**

<img src = 'https://github.com/lavsz/Mod3_Tanzania_Pump_Functionality_Prediction/blob/master/Digital_Arts/Screen%20Shot%202021-04-15%20at%205.49.28%20PM.png' width="450" height="250">

Note: most water pump has good water quality resources. 

**Would payment types affect the functionality of the pump?**

<img src = 'https://github.com/lavsz/Mod3_Tanzania_Pump_Functionality_Prediction/blob/master/Digital_Arts/Screen%20Shot%202021-04-15%20at%205.42.19%20PM.png' width="720" height="220">

Note: regular payments to the water service seems to grant better functionality

**Are there any geospatial distribution patterns?**

<img src = 'https://github.com/lavsz/Mod3_Tanzania_Pump_Functionality_Prediction/blob/master/Digital_Arts/Screen%20Shot%202021-04-15%20at%205.55.03%20PM.png' width="650" height="250">

Note: there are some regions with more non functional pumps. 

**Which regions are those?**

<img src = 'https://github.com/lavsz/Mod3_Tanzania_Pump_Functionality_Prediction/blob/master/Digital_Arts/Screen%20Shot%202021-04-15%20at%206.08.35%20PM.png'
width="600" height="300">

Regions that stood out: Lindi, Mara, Mt.Wara, Rukwa, and Tabora

## Models & Evaluation
A few different types of machine learning classifier models were utilized to study the functional status of the water pumps, including:
- Random Forest Classifier
- K-Nearest Neighbours (KNN)
- XGBoost

Random Forest and XGBoost achieved higher accuracy scores and were further tuned and evaluated. 

Final winner XGBoost classifier and the accuracy score is 79%

## Some Findings

Based on the EDA and model, some important features that affect classifying functionality include:
- Distance to the closest town (data acquired from external sources)
- Population (which infers usage)
- Height (altitude)
- Total Static head 
- Quantity
- Pemitting

## Python Libraries 
Data structuring and cleaning:
- Numpy
- Pandas
- Geopandas
- Shapely
- Math

Visualization:
- Seaborn
- Matplotlib
- Folium
- statsmodels.graphics.mosaicplot

Machine Learning:
- Sklean
- imblearn
- XGBoost

## Resources
- Detailed Jupyter Notebook is [here](https://github.com/lavsz/Module3_Final_Project/blob/master/EDA_MODEL_master.ipynb)
- The Presentation slides is [here](https://github.com/lavsz/Module3_Final_Project/blob/master/Tanzania%20Water%20Pump.pdf)

# MLE-Final-Project
Project Title: Wind Turbine Power Prediction <br>
Name: Allie Labrecque

Description: 
The goal of this project is to predict the power output from a wind turbine. The application of this  is to make wind power prediction more reliable, so that wind can account for more energy generation within a hybrid power grid. Machine learning is useful for predicting wind power because it can account for how the system behaves in the real world, rather than relying on theoretical calculations.

Dataset:
"Wind Turbine SCADA Dataset" https://www.kaggle.com/datasets/berkerisen/wind-turbine-scada-dataset
The dataset consists of data from a wind turbine collected every 10 minutes for 1 year. The features of the dataset are: Date/Time, Wind Speed (m/s), Wind Direction (°), and Theoretical Power Curve (KWh). The target is Active Power (kW).

Methods:
3 different machine learning methods were used in this project: Random Forest Regression, Support Vector Regression, and Reccurrent Neural Network. RF and SVR were chosen because they were found to be highly successful models in literature. The hyperparemeters of the RF model were tuned using GridSearch to optimize performance. RNN with LSTM was selected due to its strength in retaining information over a long period of time. 

Instructions:
Use the code in Load_Wind_Dataset.ipynb to load and filter the data, and then split it into training and testing sets. 
The file Wind_Turbine_Dataset_Visualization.ipynb contains code to visualize the different features of the dataset. 
The file 

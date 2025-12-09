# MLE-Final-Project
Project Title: Wind Turbine Power Prediction <br>
Name: Allie Labrecque

Description: <br>
The goal of this project is to predict the power output from a wind turbine. The application of this  is to make wind power prediction more reliable, so that wind can account for more energy generation within a hybrid power grid. Machine learning is useful for predicting wind power because it can account for how the system behaves in the real world, rather than relying on theoretical calculations.

Dataset: <br>
"Wind Turbine SCADA Dataset" https://www.kaggle.com/datasets/berkerisen/wind-turbine-scada-dataset
The dataset consists of data from a wind turbine collected every 10 minutes for 1 year. The features of the dataset are: Date/Time, Wind Speed (m/s), Wind Direction (°), and Theoretical Power Curve (KWh). The target is Active Power (kW).

Methods: <br>
3 different machine learning methods were used in this project: Random Forest Regression, Support Vector Regression, and Reccurrent Neural Network. RF and SVR were chosen because they were found to be highly successful models in literature. The hyperparemeters of the RF model were tuned using GridSearch to optimize performance. RNN with LSTM was selected due to its strength in retaining information over a long period of time. 

Instructions: <br>
Use the code in Load_Wind_Dataset.ipynb to load and filter the data, and then split it into training and testing sets. <br>
The file Wind_Turbine_Dataset_Visualization.ipynb contains code to visualize the different features of the dataset. <br>
The file Wind_Turbine_Project_Code.ipynb contains all of the code to run the 3 algorithims (RF, SVR, RNN), the trained models, and the plots of their results. Each section is labeled with a different header and their are text descriptions / comments explaining each step. Once the dataframe is loaded, any of the algrothims can be run independently of the others. 


Summary of results: <br>
Initially, the RF and SVR performed almost identically with R2 of 0.963 and RMSE of about 252 kW. The RF was tuned using GridSearch, but improvments were minimal. The tuned RF performed the best with R2 of 0.967 and RMSE of 237 kW. After testing with RF, it was found that that the Theoretical Power Curve feature is redundant, and that the same results can be achieved using just Wind Speed and Wind Direction. The tuned RNN performed the worse with R2 of 0.916 and RMSE of 373 kW. 

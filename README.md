# ApplianceEnergyPrediction

## Problem Statement:
The Appliances Energy Prediction dataset contains time series obtained from the Appliances Energy Prediction dataset from the UCI repository. 
The goal of this dataset is to predict the total energy usage in kWh of a house. It has temperatures in Celsius measured from the different rooms of the house and also it has the humidity percentage of the same rooms. 
Also, some additional data is added to this dataset that as temperature, humidity, wind speed, etc. from the Chivers weather station that might help predict the energy prediction. 

The main work is to predict the energy the appliances consume using these available variables. This dataset has data with a range from Jan (mid) - May, yes it has only 4.5 months of data, which may be a little difficult to accurately predict the future.
So, the main objective is to create three regression models and find their individual best by hyperparameter tuning.
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

![image](https://github.com/balaji-89/ApplianceEnergyPrediction/assets/57706260/51154bec-eafa-44fe-875c-2b44909b1198)

## What I did?:
I did EDA first to understand all the features in the dataset clearly and collect information regarding our ultimate goal model building. I find the number of total null values in the dataset and find a way to impute the null values closer to the real-world values. 
Then I going to handle outliers because these outliers disturb our model estimation. After handling outliers, I am going to add extra features which may add additional information to the model to predict with good accuracy. 
And I also have a plan to add train and add some PCA-predicted features in the dataset, which I found in Kaggle problems while working on my personal project.

After handling outliers, handling missing values, and completing feature_engineering(adding some extra features), it's time to remove unwanted features which is not useful for model building, I am going to remove the correlated features with other features and also have less impact on the target variable. 
After removing the correlated features, the next and final thing is scaling the data. Scaling is very much important for parametric tests and I going to apply the scale to the dataset for the non-parametric test too.

And finally, we will have data ready for model building. Here I am going to try three different models of SVM, one boosting algorithm and one bagging algorithm. Finally, after building the model by finding the best parameters for the model using hyperparameter tuning, I go to the same the best model's weights, so that we don't train the model again. 
This is a detailed summary of my project, which explains roughly what I am going to do.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Library Used:
  - Matplotlib, Seaborn
  - Numpy
  - Pandas
  - Sklearn

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png) 
## Execution Instructions:

1. Clone the repository:

   ```
   git clone https://github.com/balaji-89/ApplianceEnergyPrediction.git
   ```


2. Run :
      open file under src/models/ppliance_energy_ML.ipynb, then run it cell by cell
   
Feel free to modify and adapt the content according to your project's specific details and requirements.







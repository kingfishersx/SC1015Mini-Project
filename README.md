# US Traffic Accidents

## About
This mini-project for SC1015 aims to predict when traffic accidents are most likely to occur. This enables emergency services to respond quickly and efficiently to accidents during that time period.
## Data Extraction
We will be using a dataset of [US Accidents from Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents). Since this dataset is huge with more than 2.8 million records (>1 GB), we will be using ```opendatasets``` and kaggle API ("username":"testingqwerty","key": ***provided in assignment submission in NTULearn***) to download it. To avoid differences in US time zones, we will only focus on the US state of California, as it was the state with the largest number of records.  
Additionally, the original dataset has about 47 columns, but most of them like time zone are redundant so we decided to narrow our predictors down to a few most important ones like weather and temperature.

## Machine Learning models
We used the following models to predict data into 24 classes
1. Decision Tree
2. Random Forest
3. Xgboost

## Conclusion
 - The models predicted accidents to happen from 6 am to 8 am and in the late afternoons.
 - This is expected as the time periods coincide with peak hours and more cars are on the road as people travel to/from work.
 - Xgboost may not be suitable due to insufficient hyperparameter
 - Decision tree and random forest may be overfitted as accuracy of test set half of accuracy of train set
## References
 - https://www.kaggle.com/code/michaelbryantds/eda-of-vehicle-accident-data
 - https://www.kaggle.com/code/satyabrataroy/60-insights-extraction-us-accident-analysis
### Contributions
Yock Lim: ML models  
Wei Hong: Exploratory Data Analysis  
Kai Xuan: Data extraction and data cleaning  

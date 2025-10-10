# AUTHOR 
Eunice Folashade

# Technical-Test-COMP-44161

Overview
The project Automated Valuation Model to predict the assessed value of a residential property based is to assesesed property valune in winnipeg base on features  from Winnipeg assessment data using Python.It demonstrates a workflow from data cleaning to Model Explainabilty which based on below work summary.  

# Workflow Summary 

1.Data cleaning and statification : is done to remove invalid and missing entried:converted numerics types are replaced with 0
2.Feature Engineering : this added derived features like Age Ratios and defined colunms
3.Data perprocessing and Data Validatipn : Data is splitted into both test data and training Data in the ratio of 80:20 i.e the Test data is 20 and the Training data is 80 and split was done based on Accessed valued to maintain distribution across the dataset
4. Modelling : Ridge Regression , Random forest and HistGradientBoosting are choosen models for this project
5. Model selection :Models used are Ridge Rigression , Random forest and HistGradientBoosting and this project used 3 fold Cross validation on (MAE,RMSE ,R²)
6. Hyperparameter Tunning is done using RandomizedSearchCV and HalvingRandomSearchCV
7. Model Evaluation was done calculating MAE,RMSE,R²,WAPE and MAPE on the test set
8. Model Explainability by applied Aapplying SHAP Values to identify features that influences our perfomance metrics. 

# Outcomes -Non Technical Team
# Project Goal
This project is a model built to access property value in winnipeg based on features of the dataset provided for the project,by using this dataset our the model was able to learn patterns between features in the daaset to access property values . The goal of this project is to support consisted ,automated data-driven valuation  in other to access property values in Winnipeg.
# What was done
Computer models was used to learn patterns and relationships between different property features provided in the dataset.3 different models was considered and consludions was made from the result of the features thet have effect on the property value.
# Outcome
The model can predict rough estimate when accessing property value ,its not yet accurate enough for official use, but it shows what features matter most in accessing property evaluation with future improvements by adding more features for better prediction and hence deployment 
# Benefits
Property Valuation automation model process reduce manual work and human error applying sames rules to every property for consistent and fairer valuations.
It can estimates property values in seconds which speed up asssements process for business users .
It provides insight into which property features affect porperty value the most.(Word count 200)

# Outcomes -Technical Team

# AUTHOR 
Eunice Folashade

# Technical-Test-COMP-44161

Overview
The project Automated Valuation Model to predict the assessed value of a residential property based is to assesesed property valune in winnipeg base on features  from Winnipeg assessment data using Python.It demonstrates a workflow from data cleaning to Model Explainabilty which based on below work summary.  

# Workflow Summary 

.Data cleaning and statification : is done to remove invalid and missing entried:converted numerics types are replaced with 0.
 
.Exploratory Data Analysis : is done to understand and visualize the struture of the data

.Feature Engineering : this added derived features like Age Ratios and defined colunms.Data preprocessing and Data Validation was done splitting the dataset into test data and training Data in the ratio of 80:20 i.e the Test data is 20 and the Training data is 80 and split was done based on Accessed valued to maintain distribution across the dataset.

. Modelling : Ridge Regression , Random forest and HistGradientBoosting are choosen models for this project.

. Model selection :Models used are Ridge Rigression , Random forest and HistGradientBoosting and this project used 3 fold Cross validation on (MAE,RMSE ,R²).

. Hyperparameter Tunning is done using RandomizedSearchCV and HalvingRandomSearchCV

. Model Evaluation was done calculating MAE,RMSE,R²,WAPE and MAPE on the test set
 
. Model Explainability by applied Aapplying SHAP Values to identify features that influences our perfomance metrics. 


# Outcomes -Non Technical Team
# Project Goal
This project is a model built to access property value in winnipeg based on features of the dataset provided for the project,by using this dataset our the model was able to automatically value property using patterns between features in the daaset to access property values . The goal of this project is to support consisted ,automated data-driven valuation  in other to access property values in Winnipeg.
# What was done
Computer models was used to learn patterns and relationships between different property features provided in the dataset.3 different models was considered and consludions was made from the result of the features thet have effect on the property value.
# Outcome
The model can predict rough estimate when accessing property value ,its not yet accurate enough for official use, but it shows what features matter most in accessing property evaluation with future improvements by adding more features for better prediction and hence deployment 
# Benefits
Property Valuation automation model process reduce manual work and human error applying sames rules to every property for consistent and fairer valuations.
It can estimates property values in seconds which speed up asssements process for business users .
It provides insight into which property features affect porperty value the most.(Word count 200)

# Outcomes -Technical Team
# load Libraries and data ,splits data and straified sampling based on certain features.

# Exploratory Data Analysis 
To visualize the training data to gain insightusing different plots

# Feature Engineering 

Polynomial for numeric features,one-hot encoding for features,winsorized extreme outliers for property values.

#  Model Training: 

Model choosen  are Ridge Rigression , Random forest and HistGradientBoosting and  our primary model is Hisgradientboosting regressor wrapped in Transformedregressor for stable ranges.Training uses 3-fold crossvalidation based on property deciles.Final tunned parameters learning rate =0.11, max depth=9, max_leaf_nodes= 83.

# Evaluation Metrics: 
 ModeL Performance Metrics MAE:$146,084   RMSE:$1,762,157  R²:0.194  WAPE:27.74%  MAPE:3805.13%  showing that the model learned some pattern R²>0  but still struggles to generalize,prredictions have laarge variablity for extreme properties,showing that the model is not yet production ready but is a strong baseline prototype 
 
# Explainibility 
SHAP feature importance plots top features form the dataset

# Key Findings
-Model captures general patterns in assessed value but underestimate high value properties. 
-High MAPE is due to extreme outliers and long tail distribution
-Log transformation and quantile losses significantly improve mode stability
-SHAP shows that living area and land area are dominant drivers features

# Future Work
Integrate geospatial context like centroid coordinates, proximities  to amenities
Segment modelling by property type feature or neighborhood
Apply Huber loss or quantile regression for robutness
Deployment as an internal assessment dashboaard for explainability.
Track model choices ,parameter tuning and evaluation criteria.

# Tech Stack
Language :Python 3.12
Libraries: Pandas, numpy,scikit-learn,matplotlib,seaborn,shap
Environment Virtual Environment venv
Version Control Git+ GitHub

AI assistance disclosure
OpenAIchatgpt was used as a supportive tool for detecting code error.

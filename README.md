
# HR Analytics - Classifying Employees Attrition
## goals:
The main goal of this project is to get some useful information and insights about what contributes to employees feeling burnout, fatigue and attrition.
Employees attrition has a great amount of consequences to the company, and having the ability to know beforehand which employee is more proned to leave, can help mitigating some of those negative effects.
The area of Human Resource Analysis has a big weight in the field of labour market, thus expanding the knowledge about it is important.


## data sources:
the data we're about to analyze is taken from Kaggle: https://www.kaggle.com/vjchoudhary7/hr-analytics-case-study and contains a number of indicators about each Employee(N=4410), as well as his attrition status('Yes' or No).
The data contained 30 features after cleaning was done.

## Coding resources:
python version - 3

packages: pandas,datetime, numpy, sklearn, scipy, matplotlib, seaborn.

# Process

## data cleaning:
* Converted the in and out times to hours and minutes
* Created total working hours and in/out medians
* Converted numerical null values based on the median after checking their distribution

## Exploratory Data Analysis:

### Total time at work distribution:

![alt text](https://github.com/guyalmog2/HR-Analytics_Classification/blob/master/total_time_dist.png?raw=true)


### Categorical variables with respect to attrition:

![alt text](https://github.com/guyalmog2/HR-Analytics_Classification/blob/master/categorical_vars.png?raw=true)


## And here's a review of the numbers:

### For BusinessTravel :

The Attrition ratio(Yes/No) under the category Travel_Rarely is 0.175874

The Attrition ratio(Yes/No) under the category Travel_Frequently is 0.331731

The Attrition ratio(Yes/No) under the category Non-Travel is 0.086957

### For Department :

The Attrition ratio(Yes/No) under the category Sales is 0.176781

The Attrition ratio(Yes/No) under the category Research & Development is 0.186420

The Attrition ratio(Yes/No) under the category Human Resources is 0.431818

### For EducationField :

The Attrition ratio(Yes/No) under the category Life Sciences is 0.200000

The Attrition ratio(Yes/No) under the category Other is 0.138889

The Attrition ratio(Yes/No) under the category Medical is 0.192802

The Attrition ratio(Yes/No) under the category Marketing is 0.186567

The Attrition ratio(Yes/No) under the category Technical Degree is 0.128205

The Attrition ratio(Yes/No) under the category Human Resources is 0.687500

### For Gender :

The Attrition ratio(Yes/No) under the category Female is 0.180723

The Attrition ratio(Yes/No) under the category Male is 0.200000

### For JobRole :

The Attrition ratio(Yes/No) under the category Healthcare Representative is 0.169643

The Attrition ratio(Yes/No) under the category Research Scientist is 0.221757

The Attrition ratio(Yes/No) under the category Sales Executive is 0.202952

The Attrition ratio(Yes/No) under the category Human Resources is 0.155556

The Attrition ratio(Yes/No) under the category Research Director is 0.311475

The Attrition ratio(Yes/No) under the category Laboratory Technician is 0.193548

The Attrition ratio(Yes/No) under the category Manufacturing Director is 0.124031

The Attrition ratio(Yes/No) under the category Sales Representative is 0.169014

The Attrition ratio(Yes/No) under the category Manager is 0.159091

### For MaritalStatus :

The Attrition ratio(Yes/No) under the category Married is 0.142615

The Attrition ratio(Yes/No) under the category Single is 0.342857

The Attrition ratio(Yes/No) under the category Divorced is 0.112245

### For JobInvolvement :

The Attrition ratio(Yes/No) under the category 3 is 0.180952

The Attrition ratio(Yes/No) under the category 2 is 0.190476

The Attrition ratio(Yes/No) under the category 1 is 0.276923

The Attrition ratio(Yes/No) under the category 4 is 0.220339

### For PerformanceRating :

The Attrition ratio(Yes/No) under the category 3 is 0.187023

The Attrition ratio(Yes/No) under the category 4 is 0.221622

### For EnvironmentSatisfaction :

The Attrition ratio(Yes/No) under the category 3.0 is 0.158703

The Attrition ratio(Yes/No) under the category 2.0 is 0.175824

The Attrition ratio(Yes/No) under the category 4.0 is 0.156223

The Attrition ratio(Yes/No) under the category 1.0 is 0.339117

### For JobSatisfaction :

The Attrition ratio(Yes/No) under the category 4.0 is 0.128059

The Attrition ratio(Yes/No) under the category 2.0 is 0.196581

The Attrition ratio(Yes/No) under the category 1.0 is 0.297134

The Attrition ratio(Yes/No) under the category 3.0 is 0.197653

### For WorkLifeBalance :

The Attrition ratio(Yes/No) under the category 2.0 is 0.201651

The Attrition ratio(Yes/No) under the category 4.0 is 0.217158

The Attrition ratio(Yes/No) under the category 1.0 is 0.457317

The Attrition ratio(Yes/No) under the category 3.0 is 0.165946

### For JobLevel :

The Attrition ratio(Yes/No) under the category 1 is 0.183007

The Attrition ratio(Yes/No) under the category 4 is 0.191011

The Attrition ratio(Yes/No) under the category 3 is 0.172043

The Attrition ratio(Yes/No) under the category 2 is 0.216401

The Attrition ratio(Yes/No) under the category 5 is 0.150000





### Monthly income distribution with respect to attrition:



![alt text](https://github.com/guyalmog2/HR-Analytics_Classification/blob/master/Monthly_income_attritionpng.png?raw=true)



Attrition | mean | median
------------ | ------------- | -------------
0 | 65672.595296 |49300
1 | 61682.616034 |49080






### Age distribution with respect to attrition:



![alt text](https://github.com/guyalmog2/HR-Analytics_Classification/blob/master/age_dist_attritionpng.png?raw=true)



Attrition | mean | median
------------ | ------------- | -------------
0 | 37.561233 |36
1 | 33.607595 |32





### years with current manager with respect to attrition:



![alt text](https://github.com/guyalmog2/HR-Analytics_Classification/blob/master/years_current_manager.png?raw=true)



years with current manager:


Attrition | mean | median
------------ | ------------- | -------------
0 | 4.367397 |3
1 | 2.852321 |2

       	      



### Total working years years with respect to attrition:



![alt text](https://github.com/guyalmog2/HR-Analytics_Classification/blob/master/total_working_years.png?raw=true)



total working years:


Attrition | mean | median
------------ | ------------- | -------------
0 | 11.838335 |10.0
1 | 8.232068 |7.0

  	  



## Summary of the numerical variables:
### Looks like seniority plays somewhat of a role in the attrition attribute, along with total working years and years at the company, though there is a strong correlation beteen age and total working years, as well as total working years and years at the company, therefore there's a risk for multicolinearity. we'll handle it when we get to the model building.
### No observed impact among all the other variables on attrition.


## Modeling:

After scaling the data, drop some columns that seemed unimportant based on the analysis and creating dummy variables for the categirocal features, 10 models were compared to each other:
* Logistic Regression
* LinearDiscriminantAnalysis
* KNeighbor sClassifier
* Decision Tree Classifier
* Gaussian NB
* SVC
* AdaBoost Classifier
* Gradient Boosting Classifier
* Extra Trees Classifier
* Random Forest Classifier

Model	|  roc_auc(train)|	roc_auc(test_score)|	Std	| difference 
------------ | ------------- | ------------- | ------------- | -------------
LR	| 0.794988	 | 0.773722	  | 0.027442	|   0.021266 
LDA  | 0.791728	 | 0.768022	   | 0.030022	|   0.023705 
KNN | 0.845018	 | 0.628587	   |  0.011409	|   0.216431 
CART |  0.913274	 | 0.925767	   |  0.020132	|   -0.012493 
NB |  0.744253	 | 0.652894	   |   0.035116	|   0.091358 
SVM	 |  0.917756	 | 0.889239	   | 0.016506	|   0.028516 
ADA	 | 0.821872	 | 0.767593	   | 0.023960	|   0.054279 
GradientBooster	|  0.896189	 | 0.898354	   | 0.017630	|   -0.002165 
ExtraTrees | 0.992806	 | 0.989035	   | 0.001996	|   0.003771 
RandomForest | 0.985007	 | 0.979952	   | 0.005695	|   0.005055


out of the ten models, random forest and extra tree booster have shown the best results, further Grid search performed on both, with Random forest providing the best final model:
* Accuracy Score - 0.9863945578231292
* Roc_Auc Score - 0.9856921029281278



The coefficient results provided from the model were:

* med_out - 0.101722
* MonthlyIncome - 0.094801
* TotalWorkingYears - 0.093940
* total - 0.085933
* YearsAtCompany - 0.078034
* DistanceFromHome - 0.068624
* EnvironmentSatisfaction - 0.047698
* YearsSinceLastPromotion  	0.041973
* JobSatisfaction - 0.040716
* TrainingTimesLastYear - 0.039029
* WorkLifeBalance  	0.036912
* Education - 0.033316
* MaritalStatus_Single - 0.030142
* JobInvolvement - 0.029291
* BusinessTravel - 0.025486
* Gender - 0.017123
* Age_(17.958, 28.5] - 0.015844
* EducationField_Life Sciences - 0.014103
* Age_(28.5, 39.0] - 0.013945
* MaritalStatus_Married - 0.013090
* EducationField_Medical - 0.012207
* PerformanceRating - 0.011028
* Age_(39.0, 49.5] - 0.010983
* MaritalStatus_Divorced - 0.010770
* EducationField_Marketing - 0.008475
* EducationField_Human Resources - 0.006938
* Age_(49.5, 60.0] - 0.006775
* EducationField_Technical Degree - 0.006075
* EducationField_Other - 0.005028

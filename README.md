# Data-Science-Job-A-Thon 🏌️‍♀️
Analytics Vidhya 🔎 Job-A-Thon Nov 2021 | Employee Attrition Prediction 


## Problem : 

You are working as a data scientist with HR Department of a large insurance company focused on sales team attrition. Insurance sales teams help insurance companies generate new business by contacting potential customers and selling one or more types of insurance. The department generally sees high attrition and thus staffing becomes a crucial aspect.

To aid staffing, you are provided with the monthly information for a segment of employees for 2016 and 2017 and tasked to predict whether a current employee will be leaving the organization in the upcoming two quarters (01 Jan 2018 - 01 July 2018) or not, given:

Demographics of the employee (city, age, gender etc.) Tenure information (joining date, Last Date) Historical data regarding the performance of the employee (Quarterly rating, Monthly business acquired, designation, salary)

## Approach : 

🛀 *CLEANING* the Data was not much of an issue and Data only had Nan values of employee not leaving on specific day of the logs written.

_Adding Features before EDA_ <br>
- Total Number of working Months <br>
- Employee Attrited <br>
- Converting Education to variables (Master - 3, Bachelors - 2, College - 1)<br>
- Have employee got Promotion<br>
- Sum of Total Bussiness<br>
- Mean of Quraterly rating  <br>


📅 *EDA* Reviewing the Data at first we can see that 

- Employee working for the long time are not leaving the Job.<br>
- Employee Aged 21-24 and 48+ have hire attrition rates.<br>
- Employee with Relatively less salaried, left the company.<br>
- Male having higher Bussiness tend to work.<br>

👷‍♂️ *Feature Engineering*
Done One Hot Encoding of Gender and City.
Added 6 Months to the the total Working for the future Predictions 

Using Sklearn Library Trainied SVM, Logistic Regression, AdaBoostClassifier and RandomForestRegressor
Among these Model SVM with GridSearchCV Performed the Best which gave *76.78%*


*Ending Note and What Did I learn:
  - I Scored 65.05% Score on Leader Board on SVM with GridSearchCV but My earlier Predictions with Default SVM model (With Education Added in features gave 70.10% on LeaderBoard) 
  - In the code file i have not used Employee Education Feature, Initially it did gave a better results in the compitition but Final board says different
  - I could have use more effient Algorithms Like GradientBoost or CatBoost
 

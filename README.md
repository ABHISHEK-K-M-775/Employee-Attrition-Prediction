--employee attrition prediction project using Logistic Regression--

   in this project we will train a machine learning model to analyize the employee attrition using the dataset avaialable from "IBM HR Analytics Employee Attrition & Performance"

   the datset cantains varies features including numerical and categorical features
   it has 35 columns and 1470 samples 

---data preprocessing:

   >after doing visual inspection it is found that no missing values in samples ,no significant  outliers,no duplicate samples

   >few columns were dropped after noticing same values in every rows

   >visually analysed few categories which have correlation with attrition column more than 0.1



--insights observed through visual anlyzation:

  ->25 % employee who expressed strong dissagreement(1) over environmentsatisfaction are likely to quit rest are 13-11%

  ->42% and 22% Attrition rate is found in the employe who fall in age categ of <25 and 25-32 year old

  ->33% attrition rate for employee with poor JobInvolvement rating rest are 13-9%

  ->26% attrition rate with job level of 1 and <15% in rest level

  ->22% attrition rate with job satisfaction level of 1 and rest <16%

  ->24% of people who have monthlyincome <4200 are likely to attrition 17% for 7000-1000 and rest are less than 11

  ->24% of employee with stock optional level of 1 and 17% with level of 3 are likely attrition

  ->25% of employees who have less than 7 years of total working years are likely to attriation rest are <15%

  ->20% of employees who have less than 7 years at company are likely to attriation rest are <11%

  ->20% of employees who have less than 3 years at current likely to attriation rest are <11%

  ->21% employees who have less than 3 years with current manager are likely for attrition rest are <12%

--feauture engineering

  ->there are few categorical columns which are not ordinal so onehotencoding is performed on them

  ->attrition column is selected as target variable and since it is a categorical column logistic regression ML model is selected and trained on data set 


--performance of the model:

  f1_score : 58.22%
  roc_auc_score : 71.52%
  accuracy_score : 88.77%
  precision_score : 82.14%
  recall_score : 45.09%


--takeaway:

  ->while model predicts wheather a employee sample given will attrie or   not but few observations say thier need to look after employee who have strong dissagrement,poor job involvement,lowest job level,extremly low slary

  ->most importantly freshers and employees less than 27 age at high risk of exiting company, a counciling can help to understand the reason


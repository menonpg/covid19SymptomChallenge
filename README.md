# covid19SymptomChallenge Team Golden Eye:

Multivariate Regression of Current and 7-day Future-looking Deaths and Cases per Million, per Day, aggregated by US State

[Sage Betko](http://www.github.com/pkla), Rishabh Shetty, Jeff Morgan. Anne Gibbon, [Prahlad G Menon, PhD](http://www.github.com/menonpg) 
Carnegie Mellon University; Columbia University; Catholic University of America; Matri Design; University of Pittsburgh [prm44@pitt.edu]

Abstract: We develop a novel analytic approach to modeling current and future COVID-19 risk using the COVID-19 Symptom Survey data aggregated daily by State from CMU, joined with daily time-series data on confirmed cases and deaths  from the covidtracking.com project, in order to augment situational awareness of the outbreak. 
Specifically, we model current and N-day forward-looking estimates for: a) deaths per million (DPM); and b) cases per million (CPM). We find that while Facebook survey evidenced behaviors and attitudes of individual respondents collectively estimates DPM from 0 to 20 days in advance with R^2 north of 80% in out-of-sample testing, whereas the same survey data optimally predicts CPM rates 20+ days in future of a given survey. 

Scripting included:
a) ReadCMU_StateWise_COVID19SymptomsSurveyData.ipynb :  This script creates our dataset of daily aggregated CSV files of the COVID-19 Symptom Survey data by US State curated by CMU, joined with daily time-series data on confirmed cases and deaths  from the covidtracking.com project [1,2] 
b) COVID19_MultivariateModelingAndFeatureSelection.ipynb : This script develops the models that created the results which we report. 

![Results from KNN, SVM and XGBoost regression modeling of DPM and CPM N=0 to N=30 days in future](https://github.com/menonpg/covid19SymptomChallenge/raw/master/Result01.PNG)

Dataset references:
[1] Symptoms survey data aggregated by state by day: https://cmu.app.box.com/s/ymnmu3i125go4aue0qxosi3rbcae20bj ;
[2] Confirmed cases and deaths data:  https://covidtracking.com/api/v1/states/daily.json https://covidtracking.com/api/v1/us/daily.json


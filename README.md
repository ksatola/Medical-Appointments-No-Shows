# Medical Appointments No-Shows

## Overview
The goal of this project is to investigate a dataset of appoinment records for Brasil public hospitals. The data includes some attributes of patients and state if the patients showed up to appointments. The analysis should be focused on finding trends influencing patients to show or not show up to appointments. Using **descriptive statistics** the following question should be answered: What factors are important for us to know in order to predict if a patient will show up for their scheduled appointment? Predictive analytics is out of scope of this project.

The original problem description and data set can be found here: https://www.kaggle.com/joniarroba/noshowappointments/home

This project was completed as part of Udacity's [Data Analyst Nanodegree](https://eu.udacity.com/course/data-analyst-nanodegree--nd002) certification.

## Details
I have looked into the dataset and managed a few problems like unifying names, removing wrong data, adding new features based on existing data. I have also investigated most of independent variables in the dataset and made a few observations comparing them to each other as well as to the dependent one (no_show). As this was only an exploratory analysis, many potential correlations may remain uncovered. The data should be investigated further with more advanced statistical analysis to potentially reveal new insights and correlations.

For details see analysis documentation [Jupyter Notebook](https://github.com/ksatola/Medical-Appointments-No-Shows/blob/master/no-shows-ks4-final.ipynb) or [HTML](https://github.com/ksatola/Medical-Appointments-No-Shows/blob/master/no-shows-ks4-final.html).

## Findings
The most important findings are:
- Scheduling visits started on 2015-11-10 and ended on 2016-06-08.
- Visit appointments started on 2016-04-29 and ended on 2016-06-08.
- The distribution of appointments among days of week (Monday-Friday) is almost equal with a little bit less visits on Thursday and Friday. There are 24 visits on Saturday and none on Sunday.
- 10 days on average patients awaited for an appointment. 50% of patients waited up to 4 days and 75% up to 15 days for an appointment. The longest awaiting time was 179 days.
- Almost 40k patients scheduled their visit for the same day.
- Out of all patients scheduling an appointment for the same day (in total 38561), 1792 of patients did not show up (5%).
- There are many very young people in the dataset (most of them of age 0) but in general the patients age is distributed evenly and the number of patients goes drastricly down for patients older than 60 years.
- The patients are 37 years on average. 25% of patients are below 18 and most of them are below 55.
- Most of the patients are not alcoholics.
- Most of the patients are not diabetes but more than alcoholics.
- There are for handicap categories with most of the people not being handicapted.
- Most patients do not have hypertension diagnosed.
- On average, 20% of appointments were missed.
  - Out of 71831 appointments made by females, 14588 were missed with the ratio of 20%.
  - Out of 38685 appointments made by males, 7723 were missed with the ratio of 20%.
- There are patients with multiple appoinpments. The number appointments of top 10 patients range from 88 to 55. Taking into consideration, that the time range of visits appointed spans over 3 months, an appointment is most likely each examination or each specialist visit. So within one patient visit in a hospital, there could be multiple appointments scheduled. One of the no-show reasons could be the fact, that patients could be too tired to take part in all examinations during a particular visit, or the open hours were not sufficient to show up in all appointments. There could be also other reasons. The high number of appointments over so short period of time should be consulted with an SME to perform (or not) additional analysis in this area.
- For all categorical variables the distributions of show / no-show for different categories look very similar. There is no clear indication of any of these variables having bigger then others impact on show / no-show characteristics. The charts confirm about 20% no-show rate for most categories.
- The shorten awaiting period the more patients show up. Patiens scheduling appointments for the same day are much more likely to show up (ca. 17% of not showing up only).

## Statistical Analysis Scope
- Data Wrangling
- Exploratory Data Analysis (EDA)
- Examination of central tendency and spread
- Data visualizations

## Tools
- Python, libraries: numpy, pandas, matplotlib, seaborn, warnings
- Jupyter Lab

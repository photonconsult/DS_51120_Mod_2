# Mod 2 Project: Food's Gold RFP
Tom Hill

# Project:

A general store named "Food's Gold" has approached Ph[0]ton to perform an analysis on their marketing data to produce insights as to which demographic to target for their next campains.

They provided a dataset consisting of marketing data from 2012-2014 for me to explore and generate recommendations.

# Objective:

* Create a linear regression model that can predict the amount a customer will spend on wine over the next two years.

# Notes:

* Food's Gold is a fake company
* The dataset came from Kaggle and can be found here: https://www.kaggle.com/rodsaldanha/arketing-campaign
* The presentation assumes the year is 2014 and that we are identifying opportunities for Q1 2015
* These assumptions do not and did not change the results of my analysis - instead used as a storytelling device

# Process:

* Data cleaning consisted of:
1. adding missing income values with the median
2. engineering features for Education, Generation, and Marital Status
3. producing dummy variables for One-hot encoding
* Statistical tests included:
1. Anova
2. Welch's Ttest
* Linear Models used:
1. Standard
2. Polynomial
3. F-Test
4. Recursive
5. Lasso

# Libraries used:

* NumPy
* Pandas
* Matplotlib
* Seaborn
* SciPy
* Statsmodels
* Scikit Learn

# Results

*Original Training Error: 172.02446760608765

*Original Testing Error: 196.58156017150185

*Train R2 0.7328327537833788

*Test R2 0.6850644337462928

____

*Poly Training Error:  87.43126820497908 

*Poly Testing Error:  3425072180673.2207

*Train R2 0.9309861389565699 

*Test R2 -9.560390038500187e+19

____

*F-Test Training Error:  176.68838666766968 

*F-Test Testing Error:  203.70550540540967

*Train R2 0.7181495194164935 

*Test R2 0.6618248533061816

____

*Recursive Training Error:  171.87208883649276 

*Recursive Testing Error:  195.84138522503287

*Train R2 0.7381359055139782 

*Test R2 0.6661798156645562

____

*Lasso Training Error:  115.63858719809843 

*Lasso Testing Error:  195.7476059005185

*Train R2 0.7381353445435714 

*Test R2 0.666222001860492

# Winner:

* The Recursive model produced an RSME Z score of 0.52

# Technical Documentation can be found in the following notebook:

* Mod 2 Project - Food's Gold Analysis

# Presentation can be found here:

* https://github.com/photonconsult/DS_51120_Mod_2/blob/master/Foodsgold__Photon_Presentation.pdf




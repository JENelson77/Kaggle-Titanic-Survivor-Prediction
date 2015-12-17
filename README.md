# Kaggle-Titanic-Survivor-Prediction
Comparison of Machine Learning Methods.Using dplyer for data wrangling.

---
title: 'Kaggle Titanic Survivor Prediction: Comparison of Machine Learning Methods'
author: "Jim Nelson"
date: "Friday, December 11, 2015"
output: html_document
---

### OBJECTIVES
**1. Demonstrate proficiency in R.  
2. Demonstrate ability to perform appropriate data transformations and creative feature engineering.  
3. Compare performace of several R Machine Learning packages.  
4. Submit models to [Kaggle](www.kaggle.com/c/titanic) to assess performance and obtain challenge ranking.**    


### INTRODUCTION
The sinking of the RMS Titanic is one of the most infamous shipwrecks in history.  On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This sensational tragedy shocked the international community and led to better safety regulations for ships.    
One of the reasons that the shipwreck led to such loss of life was that there were not enough lifeboats for the passengers and crew. Although there was some element of luck involved in surviving the sinking, some groups of people were more likely to survive than others, such as women, children, and the upper-class.  

The goal of this study was to utilize the Kaggle Titanic Challenge dataset to perform and compare several machine learning predict analytic methods to predict which passengers survived the tragedy.  


### METHODS
### Kaggle Titanic Competition
The crowdsourcing predicitve modeling competition website Kaggle was used as a platform for this study, providing a means to assess my skills compared to other participants. As of 12/11/15 there were 3946 participants with 2458 scripts. A good description of how Kaggle works is found [here](en.wikipedia.org/wiki/Kaggle). The [Titanic competition](www.kaggle.com/c/titanic)is an active "Getting Started"competition in the "Knowledge" category which has been ongoing since September 2012.  Kaggle also makes available a forum for competition discussionand a repository for scripts and notebooks used in the competition. All Kaggle rules and instructions were followed during this study.   

### Datasets
Datasets used in this study were obtained from the [Kaggle website](www.kaggle.com/c/titanic/data) as CSV files. The "training" dataset consisted of 891 passengers with the following 12 variables: *PassengerId,Survived,Pclass,Name,Sex,Age*,  
 *SibSp,Parch,Ticket,Fare,Cabin,Embarked*. The "test"dataset contained 418 passengers and the same variables with the exception of the*Survived* variable. A complete description of the variables is shown [here](www.kaggle.com/c/titanic/data). The two datasets were combined to facilitate data curation then seperated for predicitve modeling use.In addition the following 8 vareiables were created for predictive modeling purposes *dataset, Child,	title,	familysize,	notalone,	smallfamily,	thirdClass,	SurvivedYhat*.

### Software and Computing Environment
The study was performed locally on a HP Pavilion 23 All-in-One with a 64 Bit OS running Windows 10 with 4.0 GB Ram and an AMD AP-5300 APU processor with Radeon HD graphics. The study was performed in R (R version 3.1.3 (2015-03-09) -- "Smooth Sidewalk" Platform: x86_64-w64-mingw32/x64 (64-bit))Copyright (C) 2015 The R Foundation for Statistical Computing) using the open source R platform R Studio (Version 0.98.1102 - ? 2009-2014 RStudio, Inc.)  

The following R software packages with corresponding manuals and vignettes were obtained from the The Comprehensive R Archive Network (CRAN):  
 
__Data Manipulation and Visualization:__    
   *dplyr*: A Grammar of Data Manipulation (v.0.4.3);  
   *ggplot2*: An Implementation of the Grammar of Graphics (v.1.01)    

__Logistic Regression Analysis:__    
   *glm2*: Fitting Generalized Linear Models (v. 1.1.2)    

__Classification statistics and AUROC analysis:__    
   *caret*: Classification and Regression Training (v.6.0-62);  *pROC*: Display and Analyze ROC Curves (v. 1.8)    

__Recursive Partitioning Modeling:__  
   *rpart*: Recursive Partitioning and Regression Trees (v.4.1-10);  
   *rattle*: Graphical User Interface for Data Mining in R (v.4.0.5);  
   *rpart.plot*: Plot 'rpart' Models: An Enhanced Version of 'plot.rpart'(v.1.5.3);  
   *RColorBrewer*: ColorBrewer Palettes (v 1.1-2)  

__Random Forest Modeling:__  
   *randomForest*: Breiman and Cutler's Random Forests for Classification and Regression)    

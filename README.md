# Introduction to the Healthy Communities Project

Every year the University of Wisconsin Madison publishes health data inclusing rankings and different health outcomes for every county in the United States. This project is one part of a collaborative Healthy Communities Project from the Data Science Union at UCLA in which different member chose a different health outcome to examine using the data. 

This project explores what other outcomes correlate with obesity rates and uses these findings to try to create a model that can predict a county's obesity rate using other health outcomes from the data set. 

## The Data

The dataset mainly used in the project is named Data_Sorted_through_counties. This dataset consists of relevant columns extracted from the University of Wisconsin data combined with population data from the US census. 

## Analysis

First, principal component analysis was performed to see which variables were best at predicting obesity rates. Using the findings from the PCA, two linear models were created. The first linear model used all of the variables in the datatable and the second model used only the variables that were found to predict obesity rates best from the PCA. 

## Findings

The principal component analysis using two principal components showed that the variables that best predicted obesity rates were median household income, life expectancy, and food environment index. However, the linear model using specifically these variables performed poorly, having an R-squared value of about 0.52. This means only 52% of the obesity rates could be explained by the variations in the variables in the linear model. The other linear model using all of the variables in the obesity_data dataset had better results of an R-squared value of 0.65.

## Future Improvements

The existing linear models can be improved by performing an anova analysis to better see which variables should be excluded from the model. Also, an entirely different model that is different from linear regression could show better results. 
# DSPP

OVERVIEW

This project uses 2015 data (spanning from 1998 to 2015) from San Francisco Unified School District to predict the likelihood of teacher attrition and assign risk scores to each teacher.
Analyses were performed in RStudio (R v3.3.1)

Our key question:
What factors are predictive of a teacher voluntarily resigning from the school district in a given year?

To answer this questions, we first clean our data to produce a unbalanced panel data set with one observation per teacher per year that teacher is employed. In order to enable us to accomplish a regress and round strategy after modeling, we convert all of our variables into dummies. 

Modeling and risk scores:
- We implement forward stepwise feature selection process to identify suitable variables for our model. 
- We then manually select features with an eye towards simplicity in interpretation while ensuring that our out-of-sample performance does not decline relative to the model selected in the forward stepwise process. 
- We rescale the coefficients on model to enable us to assign a risk score to every teacher


Summary and key results 
The cross-validated prediction model did not perform well on being able to predict teacher resignation.
In order to strengthen the predictive power of the model, we would want to include data on place-based factors (school factors, rental prices, distance between school and home)
These analyses provide a framework for future evaluation of this research question with additional data. 


DATA

We are unable to publish our data, as it is proprietary. 


Code:
Updated code.Rmd

PRESENTATION:
https://docs.google.com/presentation/d/14xVpjvolOsg7iS4A1i23KiCUXGJ3W4b8uY-OSfWx3aY/edit?usp=sharing

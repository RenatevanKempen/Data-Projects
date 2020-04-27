# Evictions Capstone - Summary

![image](https://user-images.githubusercontent.com/47600826/80351220-3d0af900-8872-11ea-8941-c7d2e48e4937.png)

Evictions in the USA, what is that about? According to the principle investigator at the Eviction Lab (Matthew Desmond), there are about 900,000 evictions each year, which equates to about an estimated 2.3 million people evicted, many of them children. That's about 6,300 people a day that are evicted, twice the number of people who die in car accidents every day in America. It's therefore a problem of enormous consequence in the country.
The goal of this analysis is to predict the number of evictions at county level in the USA, using different socioeconomic and demographic indicators. The data for this analysis was provided via the United States Department of Agriculture Economic Research Service and the Eviction Lab.

## Indicators
The socioeconomic indicators used in this analysis were:
-	Education level
-	Income
-	Financial burden (in this case rent)
-	Poverty rate
-	Unemployment rate

The demographic indicators used were:
-	Crude death rate - Annual number of deaths per 1,000 population. 
-	Crude birth rate - Annual number of births per 1,000 population.
-	Population
-	Information about the neighborhood

## Steps
The steps taken in the process were:
1.	Reading about the problem
2.	Initial data exploration
3.	Looking at correlations in the data
4.	Cleaning the data
5.	Modeling – trying different models to get the best

## Model
After trying different models, I’ve found the Random Forest model to work best as a predictor for evictions per county. 

## Key Insights
The key insights gained by performing this Capstone project about predicting evictions were:
-	Before cleaning any features, try to use all features as is in the model to check what the results are. If needed, you can tweak, clean, drop, rename, recategorize or reshape all features if necessary. 
-	For so many features, a simple linear regression model might not be sufficient, therefore I will start with a Random Forrest for a future project with so many not directly correlated features. 
-	If you need a positive value as an outcome, you can not just use the linear regression model, as this gives you also negative results. Better to use either a Lasso Regression or a Random Forest model to get only positive results. 
-	Running a Random Forrest can give you different results after each time you run this. Therefore I’ve chosen to submit the one with the best R^2 result. 
-	All features have a (slight) influence on the model

## Personal note
I’ll try not to forget that an eviction is not a only number. It involves people and it is probably the worst thing that can happen to anyone, as one’s home is taken away. It is more than just a place to sleep; it is a basic need, a place to feel save and welcome. 

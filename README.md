# DSND_capstone_sparkify
Churn prediction using spark. **Sparkify** is a digital music service.

## Motivation
It is not easy to attract new customers and it is even harder to keep them paying for your service. Churn rate has been one of the main issues that big companies are tackling. If we can find out the users before they churn, and positively take action to retain these users, then revenue could increase a lot in some cases.

Well, the problem is that in order to find out these users, we have to deal with huge datasets. Users behaviors generate a lot of data and it can easily surpass the capability of a single computer. So it is important that we can process the data in a distributed way.

**Spark** is the solution.

## Requirements
* matplotlib
* seaborn
* pyspark
* pyspark_dist_explore

## Files
* mini_sparkify_event_data.json: a small subset of a 12GB dataset containing users' events on Sparkify.
* 1.Data wrangling and EDA.ipynb: a jupyter notebook containing the code of cleaning the data and EDA.
* 2.Fitting and tuning.ipynb: a jupyter notebook containing the code of feature engineering and machine learning.

## Results
I have tried 3 machine learning algorithms, namely Logistic Regression, Random Forest, Gradient Boost Tree. I have chosen F1 score to evaluate the results, and Random Forest performs the best out of these 3.  
In the tuning part, it is funny that the default parameters have beaten all the pairs of parameters in the parameter grid. Anyway, I have got a model that has 0.856 as f1 score.

# Possible improvements
It is a pity that I don't have enough time to run my code on the cloud. I guess that using the full dataset could largely improve the results.  
Also, it is not easy to pick the features for fitting the model. Perhaps a more thorough study of the features could help improve the results.  
Besides, the way we define churn could be optimized too. There are other page names related to churn.

## External link
Please refer to my post on [Medium]().

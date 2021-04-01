#  Project Background

A real-estate investment company which specializes in flipping houses is looking to expand their operations across America. Their domain knowledge however lies primarily in Houston, TX, where they have existed and operated for over 20 years.

To expand rapidly, they won't have time to accumulate years of experience needed to master different cities markets, so they want to utilize technology to bridge that knowledge gap and quickly. Their first target market is Ames, Iowa.

In that vein, they have been able to acquire from Professor Dean De Cock over 2,927 observations of Housing sales in that city, which contains 23 nominal, 23 ordinal, 14 discrete, and 20 continuous features describing each house’s size, quality, area, age, and other miscellaneous attributes.

However, they have given us only 2,051 of these observations with sales prices and kept the remaining 878 sales prices hidden.

![alt text](https://ofilispeaks.com/wp-content/uploads/hypertuning.gif)

## Problem Statement

Our task is to utilize the given dataset to create a data analysis model. This model will be converted into an app to be used by this real estate company to determine key features that they shouldfocus on to increase the sales prices of houses they have flipped. They will judge the efficacy of the app through a Kaggle contest. Thus our main objectives are:

1. Identify the features in the Housing Data set that had the greatest positive or negative impact on Home Sales prices.

2. Deliver a data analysis model, that efficiently and accurately predicts sales prices.

![alt text](https://ofilispeaks.com/wp-content/uploads/Screen-Shot-2021-02-22-at-1.49.08-AM.png)

## Contents:
1. Exploratory Data Analysis
2. Graphical Visualization of Raw Data
3. Feature Engineering
4. Feature Selection
5. Model Selection
6. Hyper-Tuning Analysis
7. Conclusions and Recommendations
8. Kaggle Predictions

![alt text](https://ofilispeaks.com/wp-content/uploads/Screen-Shot-2021-02-22-at-1.49.22-AM.png)

## Conclusion and Recommendations

From what we see, it is clear that the [Overall Rating], is the most positive influential feature. But this does not give any valuable information to our client. As overall rating is an arbitrary item that means little in the real-estate (flipping) business. Below are the target features we recommend for our client:

1. **Immutable Features** These are features that our company should access before buying properties. They are immutable beacause they are very hard to change. An example is [Total Ground Living Area], we want it to be as large as possible before we buy it, because we cannot add more Ground Area without incurring heavy cost. But once we have a large Area we have serious profit potential. The top immutable features I would recommend are:

 - **Ground Living Area and Basement Size:** This is valid across most cities, the larger the Living area the more costly the house is.

 - **External Quality of the House:** This can be visualized in the Jupyter Notebook, the houses with an [excellent quality grade] sold on average for more than 350,000 USD and those with fair quality sold on average for less than 100,000 USD. So think brick versus Hardiplank.


2. **Mutable Features** These are features that can be modified, they are a profit throve for our client. Because they can buy it cheap and improve it with cheap labor to see a serious return on investment. The top mutable features we would recommend for our client to focus on in Ames, Iowa are"

 - **Kitchen Quality:** We know the saying, Kitchen sells! And it is clear that the kitchen is where we recommend our client to focus on. As we can see in the Jupyter Notebook, the better the Kitchen is, the more money a house can attract. Having just a Good Kitchen on Average sold for more than 200,000 USD, while a fair kitchen barely attracted 100,000 USD on average.
 
 ![alt text](https://ofilispeaks.com/wp-content/uploads/Screen-Shot-2021-02-22-at-1.50.09-AM.png)


3. **Neutral Features** These are features we advise our client not to spend money on. As they don't move the needle considerably. The key item we identified is:

 - **Roof Material/Type:** This had a minimal impact on Sales price, either positively or negatively. This is logical since buyers are normally intrigued by the inside and rarely view the roof.
 

4. **App Model** Looking at the performance of our models in predicting RMSE scores of unseen data. We are confident to recommend a [Linear Regression Model] that has had a [Lasso Regression] applied to it to suppress features. This [Linear Regression Model] also works best when a log is applied to skewed data. We were only able to apply this log on dependent variable [y]. Prior to applying the log, we had a predicted RMSE score of around [29,000]. Application of the log saw an improvement to about [26,000]. To further improve this model for your app, we would reccomend application of log to skewed indepented variables [x].

![alt text](https://ofilispeaks.com/wp-content/uploads/Screen-Shot-2021-02-22-at-1.49.34-AM.png)

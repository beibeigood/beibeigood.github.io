---
layout: post
title: "Casual Explanation of MLE"
date: 2021-04-06
---

Well, I guess we can go through some basic concepts while waiting. First, we need to understand what we are going to estimate by using this method. The answer is for estimating parameters of certain model. For example, consider the simple linear regression, the intercept and coefficient before independent variable are considered as parameters. Are you good with the definition?
Then, it is important to know the intuition behind maximum likelihood method. So, the parameters are calculated through the values maximizing the sample data likelihood. Remember the key point you need to be aware here is that we do entire estimation based on the observed data, and this makes sense since we are eventually choosing the parameters where data is most likely to be.
Before going any further, make sure you can tell the difference between likelihood and probability. Likelihood is the function telling us how likely we are to observe our data with given parameter values. So basically, probability aims to find the chance of certain event given a sample distribution of the data, while likelihood is to measure to what degree of sample provides support with specific parameters. Does this make sense so far?
Lastly, let us quickly review the steps of calculation. First, we can write down the joint probability distribution of sample data. Then, we just spot the maxima of the function by differentiation. Don’t forget to check for the second derivative to ensure the value you got is not minimal. One trick is that if you try to differentiate the above expression directly, you will find it hard to compute. Therefore, we often take the natural logarithm of the expression and then differentiate the log likelihood. We could do so, because the natural logarithm is a monotonically increasing function, maximizing the log likelihood is equivalent as computing the original expression directly.
Look, it’s our turn now! I hope my brief explanation help!

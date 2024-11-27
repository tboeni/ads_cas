# Day 1
## discussion
CLT (Central Limit Theorem): 
* The sample mean, x-bar, converges to a normal-distribution
* Is from hypothetical examples which are distributed in the way that the assumed distriubtion of the data is (e.g. normal, t-dist. etc)

h0:
* In (probability) statistics you want to show that the reverse of your hypothesis is unlikely to show the validity of your h0.
e.g. showing that a new school book has a better effect for the students. Try to show that using the old book has a better impact instead and reject that

Density functions:
* How to know which desinity function to use? -> depending on your theoretical distrubtion of you sample data.
One option to find the best suited one is a QQ-Plot (Quantile Quantile Plot, also used to check for normality)
X-Axis is the assumed probability per quantile and the Y-axis the real probabilty per quantile. if both match, the distribution will be a diagonal

Bionomial vs. Poisson:
* Binomial distribution is used when in an experiment something happens a fixed number of times with the same probabilities (for example a ball gets pitched by the same pitcher a number of times to the batter)
The number of successes and failures
* Poisson distrubtion is similar, but there is a continuous time interval (for example in the last 2 weeks) how many counts of an event (success/fail). For binomial it would be out of the last 20 events how many successes and failures


# Day 2

* https://wiso.education (simulation on how distributions can look very different and still fulfill the criterias of the base distribution)
* Measure of **Skewedness**: how symetrical a distribution is. Skewedness > 0 means right shift, < 0 left shift
* Measure of **Kurtosis**: how heavy the tails are. The closer to k > 0 means heavy tail and light tail < 0

* If confidence intervals are big, meaning the true value lies in a big range e.g. temperature estimation of meteo schweiz. The estimate lies in a confidence interval, and sometimes it is large. Meaning that for this specific measurement there are some variables that are not quite accurate yet (uncertainties). If convidence intervals are large (meaning the range of values is big) means that the model is yet lacking.

* Leverage plot shows how much influence a single point have on the outcome of the statistical plot/ calculations. Calculated with the **Cook's Distance**. Forecasting and intepreting data will be harder and you need to keep this in mind if you are doing analysis of the data / model. Be aware that your model was strongly influenced by such heavy leveraged outliers

* 


# Day 3

# Day 4

* Presentation about one of the test, show how it works and when it is sensible to apply with an example
* Provide example code in python with some data
* Be critical about the dataset(s) that are used, is it really showing what I want it to? Comment about any uncertainties or pitfalls
* References and literature needed perhaps?


* (Paired) Wilcoxon-Signed test: needs an odered metric scale, meaning the data needs to be able to be sorted (numeric or ordinal)
* t-test needs numerical data
* t-test (or all normailty assuming tests) tend to have lower p values since they have more assumptions about the data. Thus when the data is not normally distributed and a t-test performed it could be that the value would be misinterpreted
* The H0 of ANOVA is that the is no difference in means, which means when rejected means just that is **at least 1** mean of the groups taht is different!
* If there is no normality, instead of ANOVA we use **Kruska-Wallis-test** instead

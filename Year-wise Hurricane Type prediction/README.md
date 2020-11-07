# Polynomial Regression

## Implementation Method:

In the data part we have reduced the data from the details like wind (in knots),  pressure,longitude, latitude, day, month, year, hurricane name, hurricane number to just wind speedand year by averaging the all value of wind speed of the same hurricane in particular year.Then  using  the  Saffir-Simpson  Hurricane  Wind  Scale[1]  we  categorised  the  hurricane  andcalculated the frequency of each type of hurricane in the particular year.  On that data weapplied  Polynomial  Regression(with  2  independent  variables  year  and  hurricane  type  anddependent variable frequency of hurricane).  Then after that for choosing the model which fitsbest to data and also generalizes the performance of the model, we compute the RMSE(RootMean Square Error) on the test set to choose a good polynomial degree and plot a trainingloss vs testing loss.  For better and generalized performance of the model we also apply both __Maximum Likelihood Estimation (MLE) θ_MLE= argmax θ P(Y|φ,θ)__
and MLE does the same results as the general regression model so after adding a regulariza-tion parameter (σ2/β2)Iwhereσis noise variance (Assumptionσnot a constant) andβisvariance of some prior knowledge about parameter distribution which is known as __Maximum A Posterior (MAP) θ_MAP= argmin θ P(Y|φ,θ)P(θ)__
to estimate parameters for a distribution having a prior knowledge about parameter distribution.



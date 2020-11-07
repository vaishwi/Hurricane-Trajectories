## Dataset for dimenasionality reduction for hurricane trejectory prediction

- Data-set of Hurricane trajectory prediction contains 12 dimensions (features) and 13131 sam-ples.  So shape of data matrix X is 13131 x 12 and hereX= [x1 x2 x3..... xN]^T ∈ R^(N∗D)

- n  hurricane  trajectory  prediction  dataset,  feature  given  as  Month,  Day,  Hour,  Lati-tude, Longitude, Wind Speed, Pressure, Unique key, Distance, Direction, Grid ID whereUnique key has alpha numeric values combination of hurricane name,  year,  hurricanenumber so we separate out feature from it, as year and hurricane number.  After thatform the X which contains all the features describe above.  Datax1x2x3..... xnformsthe rows of the data matrix X where all xn has 12 feature and n=13131.  Hence forming X as 13131 x 12 data matrix.

- As we consider X= [x1x2x3..... xN]^T.  So covariance matrix is given byS=XTXwith dimensions 12 x 12.  Eigen-values and Eigen-vectors of covariance matrix S withdimensions 12 x 1 and 12 x 12 respectively.  We select 8 principle components becausevariance of data can be covered by 8 dimensions and it gives very low reconstructionerror.  So dimension of projection matrix is 8 x 8.

- If eigen values are non ordered then graph of captured variance is in random in natureso if we pick first 8 principle component then captured variance is also random in natureand result in that we may loose the data and recontruction will be not proper and thatalso affect the mean square error and also we may get very high mean square error.


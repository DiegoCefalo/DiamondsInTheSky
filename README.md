![lucy](https://github.com/DiegoCefalo/Lucy/blob/main/img/Lucy_diamonds.jpg)
# Lucy
Predicting the price of a diamond based on a couple of variables.  
I tried all of these methods from the sklearn library to create a model that predicted said price:
- PolynomialFeatures
- LinearRegression, Ridge, Lasso, ElasticNet, LassoLars, BayesianRidge, Lars, ARDRegression
- TweedieRegressor, GammaRegressor, PoissonRegressor, SGDRegressor, RANSACRegressor
- cross_val_score
- DecisionTreeRegressor
- KNeighborsRegressor, RadiusNeighborsRegressor
- GradientBoostingRegressor, RandomForestRegressor, VotingRegressor
- LinearSVR
- GaussianProcessRegressor
- KernelRidge
- PLSRegression
- MLPRegressor  
</a>
Then I tried the H2O.AutoML Library.  
After that I tried the XGBoost library with promesing results.  

Finally I used RandomSearch from sklearn and the hyperopt library to optimize the parameters of the most 3 promesing models (RandomForestRegressor, HistGradientBoostRegressor and XGBRegressor) and PolinomialFeatures (sklearn) to get every polinomial combination of the variables (max degree 2).  

The most i got was a 0.08404 of RMSE.

For a more detailed explanation please read "Explanation.ipynb" and every step I took is recorded on all the "Untitled.ipynb" in the folder "All Untitled"
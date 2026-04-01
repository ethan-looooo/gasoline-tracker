# gasoline-tracker
I worked on the exploratory data analysis including the data cleaning and visualization. I also worked on model selection and training.

Motivation
Make a finance related project without following the generic stock predictor format. Allow team members to get experience working with data and training a model.

Task
The task is to build a neural network model to predict the "Current Gas" price using the new_no_outlier.csv dataset. This involves loading the data, selecting features ('Past Week Gas', 'S&P 500', 'DOW J Oil', 'NYSE ARCA', 'DOW_NYSE_Avg', '2 Week past Gas', '3 Week past Gas') and the 'Current Gas' target, and scaling them using MinMaxScaler.

Insights or Next Steps
The established machine learning pipeline can effectively predict future gas prices. Further analysis of the MAE and MSE values from the evaluation step would provide a quantitative measure of the model's accuracy and reliability.
To move towards practical application, the trained model can be deployed as an API or integrated into a forecasting system for continuous prediction of national average gas prices, allowing for regular updates with new weekly data.

Pitfalls
The model used was a dense neural network using a rectified linear unit. This type of model is not the best at handling timeseries data which is what we used. We used 500 epochs when training which gave us a good accuracy, but may lead to overfitting issues.

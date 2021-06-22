# Moving-Average-Model-Simulation-in-Natural-Gas-Price

Continuing our simulation before, we run the simulation of Natural Gas Price using Moving Average Method. 

1. Import the dataset using pandas dataframe, adding another column which is t, that is actually the lag data (x variable). Later we calculate the residual value between Adj_Close (y variable) and t (x variable).

![pic1](https://github.com/altheanabila/Moving-Average-Model-Simulation-in-Natural-Gas-Price/blob/main/pic%201.png)


2. We use Autoregression method to test train the data. In this case we use the last 7 rows as test data while the rest is used as train data.

![pic2](https://github.com/altheanabila/Moving-Average-Model-Simulation-in-Natural-Gas-Price/blob/main/pic%202.png)


3. We need to set the model using train data as the input, and find how many lag variables after running AR method. After that, we show the lag values from the residuals.

![pic3](https://github.com/altheanabila/Moving-Average-Model-Simulation-in-Natural-Gas-Price/blob/main/pic%203.png)


4. Forecast the predicted residual values and actual values

![pic4](https://github.com/altheanabila/Moving-Average-Model-Simulation-in-Natural-Gas-Price/blob/main/pic%204.png)


5. Adding both of the values to get the real values of MA method

![pic6](https://github.com/altheanabila/Moving-Average-Model-Simulation-in-Natural-Gas-Price/blob/main/pic%206.png)


6. Calculate the mean squared error and plot the graph. As we can see the mse is getting better than previous value we got from AR method (0.004877220108676111 < 0.013473258789010692) but still has bigger value compared to Naive persistence model ( 0.004877220108676111  >  0.004342142857142858) which indicates that the time series data has a random walk problem

![pic7](https://github.com/altheanabila/Moving-Average-Model-Simulation-in-Natural-Gas-Price/blob/main/pic%207.png)

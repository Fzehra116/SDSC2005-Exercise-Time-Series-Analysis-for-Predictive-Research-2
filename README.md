# Exercise-Time-Series-Analysis-for-Predictive-Research-2

Data2: Ex4_data2.xlsx, containing the following sheets (using “Adj Close” in column F as Price for all questions below):
•	0005.hk: the price and volume of HSBC (bank)
•	0027.hk: the price and volume of Galaxy Entertainment (casino)
•	0101.hk: the price and volume of Hang Lung Properties 
•	HSI: the price and volume of Hang Seng Index (Hong Kong)
•	DJI: the price and volume of Dow Jones Index (U.S.)
•	SSEC: the price and volume of Shanghai Stock Exchange Composite (China)
•	Use linear interpolation to fill any empty cell.
Task: 
1.	ARIMA parameters: 
a.	Data: use all dates up to Dec 31, 2022 for the three stocks (HSBC, Galaxy, and Hang Lung), respectively;
b.	Use ACF (autocorrelation function) and PACF (partial autocorrelation function) to identify the autoregression (AU), integration (I), and moving average (MA) parameters for each stock price;
c.	Fit a univariate ARIMA model (i.e., only Price plus AR, I, and MA, without any IV) for each stock 

2.	Predictive models: 
a. 	Data: split the data to a training set (up to Dec 31, 2022) and a test set (from Jan 1 to Feb 21, 2023) for each stock;
b. 	Model: build a predictive model for each stocks, respectively, using Price as the DV and any of the following as the IVs:
i.	Time-effects: day of the week, month of the year (“seasonality”), and any other features that represent repeated cycles of time (see questions for Data 1); 
ii.	Internal factors: the previous price and volume of the stock (no need for previous price if you use ARIMA/SARIMA because it will be automatically included);
iii.	Market influences: the previous price of the stock market in Hong Kong (HSI), the U.S. (DJI), and mainland China (SSEC);
iv.	Optional IVs: any other time series data measured on a daily unit to be collected by you and add to the model as the IVs (same grading policy as in Data 1 applies here);
b. 	Estimation (based on the training set) and test (based on the test set) method: use any method of your choice, including an ensemble of several methods, e.g.,
i.	OLS;
ii.	Exponential smoothing;
iii.	ARIMA/SARIMA;
iv.	Machine learning/deep learning;
v.	Anything else

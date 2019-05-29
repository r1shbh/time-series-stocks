# Time Series Analysis on Stocks
Playing with NSE data from year 2015-2016 using Time Series Analysis and Bokeh Visualization.

The following tasks have been completed in the following notebook.

Dataset selection:
Use: https://github.com/swapniljariwala/nsepy
Source OCLHV data for NSE stocks (INFY,TCS) between 2015-2016. Data level - Daily.
Source OCLHV data for NIFTY IT index. Data level - Daily.
 
Part 1:

Moving Averages
Create 4,16,....,52 week moving average(closing price) for each stock and index. This should happen through a function.

Dummy series:
1. Volume shocks - If volume traded is 10% higher/lower than previous day - make a 0/1 boolean time series for shock, 0/1 dummy-coded time series for direction of shock.
2. Price shocks - If closing price at T vs T+1 has a difference > 2%, then 0/1 boolean time series for shock, 0/1 dummy-coded time series for direction of shock.
3. Pricing black swan - If closing price at T vs T+1 has a difference > 2%, then 0/1 boolean time series for shock, 0/1 dummy-coded time series for direction of shock.
4. Pricing shock without volume shock - based on points a & b - Make a 0/1 dummy time series.
 
Part 2 (data visualization ):
For this section, you can use only bokeh. https://bokeh.pydata.org/en/latest/docs/gallery.html
 
1. Create timeseries plot of close prices of stocks/indices with the following features:
2. Color timeseries in simple blue color.
3. Mark closing Pricing shock without volume shock to identify volumeless price movement.
4. Hand craft partial autocorrelation plot for each stock/index on upto all lookbacks on bokeh

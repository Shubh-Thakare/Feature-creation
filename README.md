Exponential weighted average (EWA) is a feature engineering technique used to create new features in machine learning models. The EWA technique involves taking a weighted average of past observations with an exponentially decaying weight. This technique is commonly used in time series data where the recent data points are more important than the older ones.

The basic idea behind EWA is that it assigns more weight to the more recent observations, and less weight to the older observations. This is achieved by using a decay factor that reduces the weight of past observations exponentially over time.

In the context of feature engineering, EWA is used to create new features based on the weighted average of past observations. For example, in a stock market prediction model, the EWA of the stock price over a certain period of time can be used as a new feature. This feature will capture the trend of the stock price over time and will be more informative than just using the raw stock price values.

Another example of EWA in feature engineering is in natural language processing. In this case, the EWA of the frequency of a word over a certain period of time can be used as a feature. This feature will capture the trend of the word usage over time and will be more informative than just using the raw frequency values.

Overall, EWA is a powerful feature engineering technique that can be used to capture the trend of time-series data and create informative new features for machine learning models.

Winsorizing: This technique involves replacing extreme values in the data with less extreme values. This can help reduce the impact of outliers on the data.

Binning: Binning is a technique that involves grouping continuous data into discrete categories. This can help reduce the impact of outliers and skewness in the data.


The concept of "ratio beyond 1std" in feature engineering refers to the ratio of a data point's distance from the mean to the standard deviation of the data. Specifically, a data point is said to be "beyond 1std" if its distance from the mean is greater than one standard deviation.

This ratio can be useful in feature engineering when dealing with data that contains outliers or extreme values. By using this ratio, we can identify which data points are significantly different from the rest of the data and may need to be treated differently or removed altogether.

For example, if we have a dataset of customer purchase amounts, and we find that some customers have spent significantly more than the rest of the customers, we can use the ratio beyond 1std to identify these outliers. We can then decide whether to exclude these outliers from our analysis or create a separate feature for them.

Overall, the ratio beyond 1std is a useful tool in feature engineering to help identify outliers and extreme values in a dataset.

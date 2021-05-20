# Web-traffic-prediction
Forecasting future traffic to Wikipedia pages using AUTO ARIMA.

We would be forecasting future web traffic for 145k wikipedia articles. The
given data consists of 145k wikipedia articles page and time series data is given for every page
starting from july 1st, 2015 up until September 1st, 2017. This data tells us how many views
one page is having for a particular date. Now based on these no. of views we have to predict
the no. of views which are expected for the future dates starting from September 13th, 2017
and November 13th, 2017.

Started with importing some useful libraries and loading the data. After having a
look at the data we can see that this dataset contains missing values. Even there are
some series where most of the values are missing.
Next comes the data visualization part where for more data exploration we breakdown
every page into four different columns: topic, language, access and agent type and by
the distribution plot it is shown how views are behaving with respect to each of these
features. For example what type of access(desktop or mobile) viewers are using more to
visit the site.
After that we split the data into train validation sets. 
Removed outliers using 'IsolationForest'. 
Trained AUTOARIMA on the dataset after removing outliers. 

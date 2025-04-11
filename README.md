# Click Through Rate Prediction

The project aims to use XGBoost to predict the click through rate (CTR) for Avazu, a company providing services of online advertising and digital marketing. CTR is one of the key factors in business valuation. Improving the accuracy of CTR prediction is important because if the application has a large user base, a small improvement in CTR prediction could result in a large increase in revenue. On the other hand, in real-time bidding systems, CTR is used to determine which ads win auctions and at what price, so more accurate predictions lead to better matching between ads and users.


## Project Structure

`data/': The dataset is from https://www.kaggle.com/c/avazu-ctr-prediction/data. The dataset contains 11 days of Avazu data including user clicking behavior, when and where a user clicked the advertisement.

`Click_Through_Rate_Prediction.ipynb': The Jupyter notebook has codes for data exploration, feature pre-processing, model training and evaluation.

`images/': The folder contains data visualization and figures of model evaluation.

## Data Exploration

The dataset provides several named and anonymous features. All features are categorical, and I use bar charts to compare the distribution of click behavior among categories for each named feature. The overal click through rate was 16.98%, which was pretty high. The click through rate varies over time in a day, and it was highest in the afternoon. Banner position is one of the most important factors that affect click through rate of an advertisement. The data shows the ads placed at banner position 7 were most likely to be clicked, while banner position 2 seemed to yield the lowest click through rate. I also gain insights for effective marketing by examining click behavior across device type. Site, App

![Click Proportion](images/Click_dist.png)
![Click Distribution by Hour](images/Click_hour.png)
![Click Distribution by Banner Position](images/Click_banner_pos.png)
![Click Distribution by Device Type](images/Click_device_type.png)
![Clcik Distribution by App Category](images/Click_app_cat.png)
![Clcik Distribution by Site Category](images/Click_site_cat.png)
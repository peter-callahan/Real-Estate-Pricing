# 51-callahan-mlproj-realestate

## Goal

This project seeks to create a price prediction mechanism for real estate listings using historical transaction data.  A secondary goal is to idenify pricing markets based on property features and through data enrichment to reveal new insights for real estate markets.  This analysis will focus on residential real estate. 

Due to the challenges finding complete datasources this analysis will incorporate historical data to the extent it can be obtained.  Currently data is available back to ~2001 in some markets and this project will seek to incorporate that data after normalizing for inflation. Though it is not possible to account for all market dynamics (and dysfunction) converting price data to 2022 dollars will provide more datapoints with which to train a prediction model.

## Metrics: 

### Predicted Price  
The model should predict the value (price) of an individual property based on the parameters of the property.  These predictions can be checked for accuracy using RMSE as they will be decimal values.  Predicting price is important as it will identify pricing opportunities for open listings that are too low.  The business context is that these low priced values represent opportunities for my fictional real estate business.  The model will be considered "good enough" when normalized RMSE is below 20%.  Normalized RMSE is discussed more here: https://www.statology.org/what-is-a-good-rmse/

### Market Clusters  
Clustering accuracy in this case will be difficult since there will not be a ground-truth with which to compare the model.  Instead, the insights from clustering will need to make sense given real world examples.  For example, clusters should identify neighborhood boundaries not captured formally, such as with zip codes.  Researchers could map these clusters against areas where known boundaries exist to see if the model can identify those boundaries. Examples include areas where physical obstacles (train tracks, highway) seperate neighborhoods of different demographics or areas of large homogenous political and economic demographics.

## Appendix: 
1. https://www.kaggle.com/datasets?search=real+estate
2. https://catalog.data.gov/dataset?q=Housing+for+sale&sort=score+desc%2C+name+asc&tags=housing
3. https://realtyna.com/blog/what-are-best-public-sources-real-estate-data/

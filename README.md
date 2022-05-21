# 51-callahan-mlproj-realestate

## Goal

> Comment from Daniel: I think this is a great idea for a project, especially with the way the housing market has been recently. Will your model somehow take in the current state of the market where everything tends to be more expensive? Also how far back in time do you plan to look at historical data?

This project seeks to create a price prediction mechanism for real estate listings using historical transaction data.  A secondary goal is to idenify pricing markets based on property features and through data enrichment to reveal new insights for real estate markets.  This analysis will focus on residential real estate.

## Metrics: 

> Comment from Daniel: It may be a good idea to have a target accuracy for the model. This way you have a concrete stopping point for when the model is "good enough"

### Predicted Price  
The model should predict the value (price) of an individual property based on the parameters of the property.  These predictions can be checked for accuracy using RMSE as they will be decimal values.  Predicting price is important as it will identify pricing opportunities for open listings that are too low.  The business context is that these low priced values represent opportunities for my fictional real estate business.   

### Market Clusters  
Clustering accuracy in this case will be difficult since there will not be a ground-truth with which to compare the model.  Instead, the insights from clustering will need to make sense given real world examples.  For example, clusters should identify neighborhood boundaries not captured formally, such as with zip codes.  Researchers could map these clusters against areas where known boundaries exist to see if the model can identify those boundaries. Examples include areas where physical obstacles (train tracks, highway) seperate neighborhoods of different demographics or areas of large homogenous political and economic demographics.

## Appendix: 
1. https://www.kaggle.com/datasets?search=real+estate
2. https://catalog.data.gov/dataset?q=Housing+for+sale&sort=score+desc%2C+name+asc&tags=housing
3. https://realtyna.com/blog/what-are-best-public-sources-real-estate-data/

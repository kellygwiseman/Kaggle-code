Africa_Soil_Property-competition
================================

Digital mapping of soil functional properties, especially in data sparse regions such as Africa, is important for planning sustainable agricultural intensification and natural resources management.   For this Kaggle competition, we were asked to submit the predicted values for five target soil functional properties - Ca, pH, P, SOC, and Sand - using mid-infrared absorbance measurements and remote sensing spatial data.

The trickiest part of this Kaggle challenge was avoiding over-fitting the training data. Only 13% of the test data, out of a small 727 sample set, were used to calculate the Kaggle public score. In addition, there were more features (3,580) than training samples (1,157). I found that Support Vector Regression was a good method for modeling this data set with a large feature to sample ratio.

This Ipython notebook contains all of the code I used for this Kaggle competition. A summary of this project can be found at http://www.kellygwiseman.com/#!africa-soil-property-challenge/c1xgw.
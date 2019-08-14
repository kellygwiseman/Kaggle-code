Restaurant Revenue Competition
=====================

With over 1,200 quick service restaurants across the globe, TFI is the company behind some of the world's most well-known brands: Burger King, Sbarro, Popeyes, Usta Donerci, and Arby’s. They employ over 20,000 people in Europe and Asia and make significant daily investments in developing new restaurant sites.

Right now, deciding when and where to open new restaurants is largely a subjective process based on the personal judgement and experience of development teams. This subjective data is difficult to accurately extrapolate across geographies and cultures.

For the competition, we were to submit the predicted annual revenue for each of the test restaurants. Submissions are evaluated using the root mean squared error.

The competition had two main challenges: (1) obfuscated data fields and (2) small training set. I tested treating all the obfuscated fields as categorical features, treating them all as ordinal/numeric features, and a few combinations of the two. What performed best during cross-validation was treating the fields that had an absolute correlation with revenue of at least 0.1 as ordinal/numeric and treating the rest of the obfuscated fields as categorical. My approach to the small training set was to reduce the number of features and use relatively simple models to avoid over-fitting the data. I chose to average the predictions from a ridge regression model and support-vector regression model. Since there were many more cities in the test set than in the training set, I decided not to use it as a feature. This reduced the feature space significantly. For the ridge regression model, I reduced the feature space further using kernel princicpal component analysis. 

This Ipython notebook contains all of the code I used for this Kaggle competition.
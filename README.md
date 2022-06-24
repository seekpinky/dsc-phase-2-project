

## Project Overview

For this project, you will use multiple linear regression modeling to analyze house sales in a northwestern county.

### Business Problem
ABC company interest to buy property in King County. Their budget is around 500K dollars. They are new to the area, and interest about the housing in Seattle. They want to decide if they should buy property in Seattle or other area within King County.

### The Data

This project uses the King County House Sales dataset,`kc_house_data.csv`, found in the data folder in this repository. The description of the column names for the data set can be found in jupyter notebook.

### Train-Test Split.
Train- Test set is pefromed to the data. 75% of the data is split into the train set and 25% of the data is split into test set. Also, target variable, price is seperated into y_train and y_set with the same ratio.

### Data cleaning and Preprocessing
OLS analysis only take data type in numerical form (int64 or float64). We need to change the categotical data into numerical form.  We need to identify categorical nominal variable and categotical oridnal variable.
Those include: floors, sqft_basement, view, condition, grade, ,
Improper data type is found in sqft_basement. The improper data is replaced with mean of the sqft_basement, and the datatype is change to float afterwards.
Missing value also found in waterfront, yr_renovated, view is found. Missing value is replaced, and yr_renovated is replaced by is_renovated with 0 or 1 as is renovated n not renovated instead.

### Mehods.
3 Linear Regression were performed for this analysis

### Baseline Method.
Every factors from the data set were ised as predictors.

R2 train score to .87
R2 test score to .85

### Linear Regression Method with VIF.
Only 35 predictors is used for analyzing as Variance inflation factor reduce the multicollinary facor between factors.
Criteia is VIF score <5.

R2 train score to .69
R2 test score to .66

### Linear Regression Method with VIF with outliers removed. New data set is created with additional 3 cities column
Outliers are removed for several predictors. Test_train split has to be performed to create another set of data: (x_train1, x_test1, y_train1, y_test1). Data cleaning and pre-processing are followed from the procedure above to create data. Also, 3 different column name seattle, kent, and  Bellevue by grouping the zipcode that they belong.

R2 train score to .65
R2 test score to .63

### Comparison between home sale prices between Seattle, Kent, Belleube


### Recommendation
ABC comapny budget should be able to fit the houses in Seattle. However, I would suggest they should look into property in Kent as houses are cheaper and nicer in Kent compare to Seattle.

Rather focus on property itself as Square footage of the apartments interior living space, Square footage of the land space,Number of bedrooms and Number of bathrooms are top factors that correlated to the sellilng price.

### Next Step
Further investigate the relationship between individual predictor and outcome as they may not have a linear relationship.

Continue to collect data for house sale during covid to see if factor changes as people work from home

Adjust house sale price for inflation. We may get a more accurate analysis

Collect additional data for the upcoming year and more as recession is coming.

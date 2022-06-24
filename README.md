
![awesome](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-2-project-v2-3/main/halfway-there.gif)

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



### Recommendation

### Next Step
Further investigate the relationship between individual predictor and outcome as they may not have a linear relationship.

Continue to collect data for house sale during covid to see if factor changes as people work from home

Adjust house sale price for inflation. We may get a more accurate analysis

Collect additional data for the upcoming year and more as recession is coming.

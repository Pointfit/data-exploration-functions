# Functions

## Metadata Extraction

### `metadata(df)`
Returns column metadata including column name, data type, percentage of missing values, number of unique values, and basic statistics for interval columns.

## Data Exploration

### `data_exploration(df, column)`
Creates plots for unique values of categorical variables with less than 10 unique values. For numerical variables, it identifies outliers, creates box plots, and plots interval column distribution by decile.

## Categorical Data Visualization

### `pie_cate(df, column)`
Generates a pie chart displaying the frequency distribution of a categorical variable.

## Stability Chart

### `stable_chart(lift_table)`
Plots a captured response rate plot based on the provided lift table.

## Feature Selection Methods

### `forward_selection(X, y, significance_level=0.05)`
Performs forward selection to identify the best features based on the significance level.

### `backward_elimination(X, y, significance_level=0.05)`
Performs backward elimination to identify the best features based on the significance level.

### `stepwise_selection(X, y, significance_level=0.05)`
Combines forward and backward selection to identify the best features iteratively.

## Model Summary

### `enter_selection_method(X, y)`
Fits an OLS regression model with all predictors and returns the model summary.

## Hosmer-Lemeshow Goodness-of-Fit Test

### `hosmer_lemeshow_test(y_true, y_pred_probs, n_bins=10)`
Performs the Hosmer-Lemeshow Goodness-of-Fit Test for logistic regression models and returns the test statistic and p-value.

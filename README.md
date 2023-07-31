# KNN-Imputation-Method
- K-Nearest Neighbor imputation <br/>
- a method used to fill missing values in a dataset by using the values of its K-nearest neighbors <br/>
- leverages the similarity between data points to estimate the missing values <br/>
- widely used in data pre-processing, especially in continuous or numerical data <br/>
<br/>

## Steps in KNN imputation method <br/>
1. Identify missing values <br/>
2. Calculate the similarity or distance between data points <br/>
    - Common distance metric: Euclidean distance, Manhattan Distance, or Pearson correlation, etc. <br/>
3. Select k <br/>
    - k = no. of nearest neighbors to consider <br/>
    - Typically, k is set to an odd no. to avoid ties when taking a vote for imputing <br/>
4. Find nearest neighbors <br/>
5. Impute missing value <br/>
    - Imputed value for missing data is calculated by averaging or taking the weighted average of the values of its k-nearest neighbors <br/>
    - For numerical data ⇒ mean or median of the neighbor’s values <br/>
    - For categorical data ⇒ majority vote <br/>
6. Repeat for all missing values <br/>
7. Repeat the process <br/>
<br/>
<aside>
💡 Choice of ‘k’ can significantly impact the imputation results. <br/>
💡 Smaller k may lead to noisy imputation, while larger ‘ might smooth out the data too much. <br/>
💡 Optimal k-value can be determined using cross-validation or other performance evaluation techniques. <br/>

</aside>
<br/>
<aside>
💡 KNN imputation is computationally more intensive, especially for large datasets, as it calculates distances between data points. Thus, it might not be the most efficient choice for very large datasets.

</aside>
<br/>

Ref : <link>https://machinelearningmastery.com/knn-imputation-for-missing-values-in-machine-learning/</link>

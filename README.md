# Feature Engineering

<h4> A process of extracting useful features from raw data using Maths, Statisics, Domain knowledge.</h4>

Feature engineering helps in data cleaning,
We do feature engineering before the data is put in machine learning model

[Feature Engineering Kaggle](https://www.kaggle.com/code/ryanholbrook/what-is-feature-engineering)<br/>
[EDA, Step by step](https://www.simplilearn.com/tutorials/data-analytics-tutorial/exploratory-data-analysis)<br/>
[Data Cleaning](https://towardsdatascience.com/what-is-feature-engineering-importance-tools-and-techniques-for-machine-learning-2080b0269f10)<br/>
[Kaggle data cleaning course and codes](https://www.kaggle.com/learn/data-cleaning)<br />
[IBM_DataCleaning_Lab](https://www.coursera.org/learn/ibm-exploratory-data-analysis-for-machine-learning/ungradedLti/qfAqI/practice-lab-data-cleaning)


![dataCleaning2](https://user-images.githubusercontent.com/33677647/201374239-ca5f3c23-ae74-4275-b413-6bf760090caf.jpg)

some of its examples are

- Outlier detection
- Imputation = the process of replacing missing data with substituted values.  Handling missing values
- Feature encoding (One hot encoding) 
- Feature creation = Two features as one, saves time, memory, Price and sq.ft --> price/sq.ft
- Feature transformation
- Feature Scaling
- Check (If we intend to use linear regression as our model, then we need to check if there is linear relation btw. our features or not).

![a](https://user-images.githubusercontent.com/33677647/201405617-ec201038-2140-4521-b289-e39ef17b9207.JPG)

### Check Linear Relation if intended 

So an example of a linear model relating a feature variables x1, variables x1 and x2 with a target label variable y, is what we see here. The function of x equals beta naught, some intercepts, plus some coefficient beta 1 times x1 plus another coefficient beta 2 plus x2. And here beta, beta naught, beta 1, beta 2 are going to be the parameters that we will hopefully learn with our model. An example that you can think of is, what we'll use also in the later graphs, is box office returns. And you can think of x1 as the cast budget and x2 as the marketing budget. And then beta 1 and beta 2 determining how much the cast budget and the marketing budget will actually help in predicting what the revenue will be for that movie.
 
we can actually transform each one of these parameters to ensure a linear relationship. 
**i.e log transformations can be a useful way to find a linear relationship when the underlying raw data may not actually have a linear relationship.**

### Feature Transformation (Transformation of distribution of data / to make linear relationship between features)

For linear regression, we assue that our residuals are normally distributed. But often raw data and target predicted feature is skewed,
log transformations can be a useful way to find a linear relationship when the underlying raw data may not actually have a linear relationship.
 
![a](https://user-images.githubusercontent.com/33677647/201408901-9f0fec30-949b-4479-8d5b-57ee6216564e.JPG)

some libraries to transfom data :
- **log and log1p** from NumPy. log1p is just going to be log, except you add one because you can't take the log of zero, so in case you have zero in your data set. 
[I used log to transform data in this Lab](https://github.com/sundas586/Data_Cleaning/blob/main/DataCleaning_IBM_DataScience.py)
- **boxcox** is just a more complex way to find the ideal way to transform from a skewed data set to a normal distribution
  
![a](https://user-images.githubusercontent.com/33677647/201416157-c261e892-7fd3-4261-b267-b4d29d4a1c32.JPG)



 
 

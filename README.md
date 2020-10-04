<img src="https://raw.githubusercontent.com/codecaviar/digital_asset_management/master/assets/bingyune-and-company-logo-6400x3600.png" align="left" width="200" height="auto">

<br/><br/><br/><br/>

----------

# Unknown Diabetes Risk: What to Do with Missing Data Values

**Code Caviar Story**: https://www.bingyune.com/blog/diabetes-risk-missing

## Project Overview

Missing data (or missing values) is defined as the data value that is not stored for a variable in the observation of interest. The problem of missing data is relatively common in almost all data science problems and can have a significant effect on the conclusions that can be drawn from machine learning models. Most datasets have missing values, and the likelihood of having missing values increases with the size of the dataset. In general, there are three types of missing data: 1) Missing completely at random (i.e. not systematic, missing data is just a random subset of the data); 2) Missing at Random (i.e. systematic, missing data is conditional on another observed variable); and 3) Missing Not at Random (i.e. non-ignorable and problematic, missing data mechanism has to be modeled). The first step in diagnosing randomness of the missing data is to use your substantive scientific knowledge of the data and your field. The second step is knowing how to identify, remove, and impute missing values as needed.

**The goal of this project is** to provide a Quick Guide on best practices to handle data with missing values. The project makes use of the Pima Indians Diabetes Database from [Kaggle](https://www.kaggle.com/uciml/pima-indians-diabetes-database). The dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The dataset was created to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. A key constraint of the dataset is that all patients identify as female at least 21 years old of Pima Indian heritage. There are a total of 768 observations and 9 variables

## Summary:

In real world data, there are often cases where a particular observation is missing because of various reasons, such as invalid or corrupt values. The handling of missing data is very important during the preprocessing of the dataset as many machine learning algorithms do not support missing values. When it comes to machine learning with Python, missing values can be handled in many different ways (each with its own pros and cons). For instance, deleting the rows or columns having null values is a simple technique, but you also lose a lot of information. Alternatively, columns in the dataset with numeric continuous values can be replaced with the mean, median, or a constant of remaining values in the column. When the missing values are from categorical columns (string), the missing values can be replaced with the most frequent category in the column. More advanced methods use either a classification or regression model to predict missing values depending on nature of the feature having a missing value. Lastly, having a domain knowledge about the dataset is also important because making the right decision on how to handle missing values generates more robust data models and better conclusions.

## Getting Started

Cloning the git repository and installing the provided packages will help you get a copy of the project up and running on your local machine. The analysis for this project was performed using Jupyter Notebook (.ipynb) and the packages were managed using the Anaconda platform.

```
git clone https://github.com/codecaviar/diabetes_risk_missing.git
conda env create -f environment.yml
```

File Description:
* environment.yml - packages used to perform this analysis  
* diabetes.csv -  Pima Indians Diabetes Database from Kaggle
* notebook_diabetes_risk_missing.ipynb - Jupyter Notebook for this project including examples and explanations

## Authors

- **BingYune Chen** - [LinkedIn](https://www.linkedin.com/in/bingyune-chen/)
- **BingYune & Co** - [GitHub](https://github.com/codecaviar)

## License

The project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

The project referenced the following resources:
* https://towardsdatascience.com/7-ways-to-handle-missing-values-in-machine-learning-1a6326adf79e
* https://towardsdatascience.com/easy-data-science-with-r-and-python-diabetes-among-the-pima-indians-an-exploratory-analysis-d7bc321d0fa7
* https://machinelearningmastery.com/handle-missing-data-python/
* https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-017-0442-1

----------
The Code Caviar is a digital magazine about data science and analytics that dives deep into key topics, so you can experience the thrill of solving at scale.

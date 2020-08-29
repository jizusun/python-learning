# Python Learning



https://github.com/jizusun/python-learning



https://www.linkedin.com/learning/python-programming-efficiently/install-anaconda-python-distribution?u=57692769



- shift+enter: execute

  

https://www.linkedin.com/learning/python-for-data-science-essential-training-part-1/introduction-to-the-data-professions?u=57692769

- Python3.6 

- Anaconda 

- Familiarity with Jupyter notebooks



## Introduction to the Data Professiionals

Course Roadmap

- Introduction to the Data Professions
- Data Preparation Basics
- Data Visualization 101
- Practical Data Visualization
- Basic Math and Satistics
- Data Sourcing via Web Scraping
- Building Collaborative Analytics plotly



Generate Business Value from data

- Data science
- Data engineering
- Data analytics
- Business intellligence



Artificial Intelligence 

- Prediction - predictive modeling (from data science)
- Execution - autonomous response (from engineering)

Programming language

- Python
- R
- Go
- Julia

Main Python Libraries for Data Science

- Advanced Data Analysis

  - Numpy
  - SciPy
  - pandas

- Data Visualization

  - Matplotlib
  - Seaborn

- Machine Learning

  - Scikit-learn
  - TensorFlow
  - Keras

  

Pandas

- A set of square-brackets[...]
- The .loc[] indexer

### Data Preparation Basics

- Filtering and Selecting

```python
series_obj = Series(np.arange(8), index = ['row 1', 'row 2', 'row 3',  'row 4',  'row 5',  'row 6',  'row 7',  'row 8'])
series_obj

DF_obj.loc[['row 2', 'row 5'], ['column 5', 'column 2']]

series_obj['row 7']

series_obj[[0, 7]]

series_obj['row 3': 'row 7']

DF_obj < .2

series_obj[series_obj > 6]

series_obj['row 1', 'row 5', 'row 8'] = 8
series_obj
```

- Treating missing values

  NaN : Not a Number

  - Figuring out what data is missing

  ```python
  missing = np.nan
  series_obj = Series(['row 1', 'row 2', missing, 'row 4', 'row 5', 'row 6', missing, 'row 8'])
  series_obj
  series_obj.isnull()
  ```

- Filling in for missing values  

```python
np.random.seed(25)
DF_obj = DataFrame(np.random.rand(36).reshape(6,6))
DF_obj

DF_obj.loc[3:5, 0] = missing
DF_obj.loc[1:4, 5] = missing
DF_obj

filled_DF = DF_obj.fillna(0)
filled_DF

fill_DF = DF_obj.fillna(method='ffill')
fill_DF
```

- Counting missing values

```python
np.random.seed(25)
DF_obj = DataFrame(np.random.rand(36).reshape(6,6))
DF_obj.loc[3:5, 0] = missing
DF_obj.loc[1:4, 5] = missing
DF_obj

DF_obj.isnull().sum()

```

- Filtering out missing values

```python
DF_no_NaN = DF_obj.dropna()
DF_no_NaN

DF_no_NaN = DF_obj.dropna(axis=1)
DF_no_NaN
```



### Data Visualization 101 

### Practical Data Visualization

### Basic Math and Statistics 

### Data Sourcing via Web Scraping

### Collaborative Analysis with Plotly












# EDA-Pandas_Profiling
Exploratory Data Analysis using Pandas Profiling Library

# Exploratory Data Analysis (EDA) 
Indeed is the first and one of the most important steps for all the data scientists. It is quite hard to imagine a model without EDA. Firstly, I would like to give a single line understanding of what EDA is. EDA gives us more insight into the data such as missing values, duplicates, count, mean, median, quantiles, distribution of data, correlation of variables with each other, type, etc. Well, we already have many good packages such as describe(), info(), isnull(), etc, which gives a neat analysis of our data. This sometimes might get us into too much of coding and is time taking, too. A question might arise- “Don’t we have a better and faster way for EDA in a very short time?” And the answer is- “Yes, we do.” There is a package called ‘Pandas Profiling’ with which we can have much analysis with just a single line code. It returns a report in the interactive HTML format which is quite easy to access and analyze the data.

## Installation of Pandas Profiling using PIP
pip install pandas-profiling

## Installation with the conda package
conda install -c conda-forge pandas-profiling

## Pandas-Profiling is divided in 5 Sections
- ### Overview
- ### Variables
- ### Correlations
- ### Missing Values
- ### Sample

### 1. 

Overview Section: 
The overview section provides overall data set information. This section has 2 sub-sections namely ‘Dataset info’ and ‘Variables types’.
Dataset info sub-section displays several variables (columns), several observations (rows), missing cells, duplicate rows, total size, etc.
Variables Types sub-section displays types of features like how many features are of numeric type, how many are of categorical type, boolean, date, URL, text (Unique), rejected, unsupported. Besides, it even displays ‘Warnings’ where it gives which feature(s) are highly correlated to others and which have a maximum percentage of 0s.

### 2. Variable Section: 
Variables section provides the information of every feature individually unlike Overview sections which provides information on the whole data set. It provides information like unique points and its percentage; missing values and its percentage. Also, as we can see on the right side, it gives a minimum and maximum values, and the percentage of zeros in that feature. If we click on the Toggle details option as shown in the above image, the new section shows up. Refer to the below image for a new section (Toggle details).

### 3. Correlation section: 
Correlation section provides a visualization of how features are correlated to each other with seaborn’s heatmap. We can have a clear and easy understanding of how features are correlated with each other. Referring to the highlight in the above image (Correlation section), we can easily toggle between different correlations like Pearson, Spearman, Kendall, and phik.

### 4. Missing value:
This section provides two graphs ‘Matrix’ and ‘Count’.
In the Matrix graph, we can visualize missing values. From the left graph, we can conclude that there are no missing values.
In the Count graph, we can visualize the count of data points in each feature. From the left graph, we can conclude that all the features have the same count of data points.

### 5. Sample Section: 
This section displays 1st 10 data points (head of 10) and the bottom 10 data points (tail of 10).

# The-Data-Analysis-Process
Automated codesets to analyse any dataset and generate insights from the same
1. Data Cleansing 

2. Metadata Preparation 
Code written to assign folder path and get a csv output in this form for every variable in the datasets

Prior to using the code, the path to the directory would need to be changed and the code detects all the csv files in that folder and creates an appended metadata for all automatically. The file can be easily identified by the 'filename' column. 
The code does the following :
- Metadata Preparation
- Information about data type with missing value
- Descriptive summaries
- Outlier detection

3. Exploratory Data Analysis
a) Univariate Analysis
Typical variable types and ideal plots to depict their distribution -
Categorical variables: Look for deviations from rank frequency distribution 
Plot rank vs frequency in descending order of log-log graph 
Ordered categorical variables: Look for distribution, multimodality, spikes, gaps, outliers - 
Plot rank vs frequency in log-log graph
Continuous variables: bin it and look for type of distribution, multimodality, spikes, gaps, outliers 
Frequency histogram in log y scale
Perform discussed analysis for all columns on Star data, Railways data(FOIS and dataset on public gramener) - Juhi
Perform discussed analysis for all columns on Parliament, Insurance and SSA data - satheesh

b) Bivariate analysis:
Say, m categorical variables, n numeric variables  
Categorical vs categorical : Contingency Table/Cross Tabs - matrix ( 3 dimension ) 
Chi-squared test : to validate results 
A note: A comparison of the expected to the actual shows insights for such plots. Try and group similar deviations by ordering the categorical variables using hierarchical clustering. The distance metric is the correlation of deviations. (I'm sure this makes no sense. Contact Anand.)
Visualization - Heat Map 
Number of possibilities - (m*(m-1))/2
Categorical vs numeric : Group Means Analysis - distribution analysis
2 samples - t test
Visualization - Tree Map, Bar Chart
Numeric vs Numeric : Correlation matrix - to understand how numeric variables  are related with each other
Visualization - Cluster Plot
Number of possiblities : (n*(n-1))/2

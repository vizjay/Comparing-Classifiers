# Comparing-Classifiers
The goal of this project is to use various classifiers to predict whether the customer will subscribe to a bank term deposit. The target variable y would be 'yes' if the customer subscribes. Else 'no'.

#### High level data tasks: <br>
&nbsp;&nbsp;&nbsp; 1) Pull the dataset into a dataframe for analysis. <br>
&nbsp;&nbsp;&nbsp; 2) Look at data description to understand missing values and basic statistics of each feature. <br>
&nbsp;&nbsp;&nbsp; 3) Plot Categorical and Numeric features to understand its distribution.<br>
&nbsp;&nbsp;&nbsp; 4) Transform numeric features by standardizing it as needed. <br>
&nbsp;&nbsp;&nbsp; 5) Transform numeric features to numeric data. <br>
&nbsp;&nbsp;&nbsp; 6) Encode categorical features. <br>
&nbsp;&nbsp;&nbsp; 7) Reduce cardinality of features having a large number of unique values
&nbsp;&nbsp;&nbsp; 8) Perform <b> K Nearest Neighbor </b>, <b>Decision Trees</b> and <b>Support Vector Machines</b> classification on transformed data with <b>y</b> as target variable.

#### Data Understanding:
&nbsp;&nbsp;&nbsp; 1) <b>Acquire data</b> - Data has been aquired from UCI Machine Learning at https://archive.ics.uci.edu/dataset/222/bank+marketing.<br>
&nbsp;&nbsp;&nbsp; 2)<b> Data description</b> - The dataset contains 41188 rows with 20 independent variables and one dependent variable. The format of raw data is a .csv file. The target variable of the dataset is the column <b>"y"</b>. </br>
&nbsp;&nbsp;&nbsp; 3) <b>Data quality</b> - There are no missing data in any of the columns.. </br>

#### Data Preparation:
&nbsp;&nbsp;&nbsp; 1)<b>Data Cleanup</b> - Column <b>"Day of the week"</b> has no impact on the subscrition rate. So this column is dropped. Also, there are duplicate records that were dropped.
Majority of the value for feature <b>"poutcome"</b> doesn't denote a success or failure based on the previous marketing campaign. Therefore this column is also removed.

#### Remove Outliers:
&nbsp;&nbsp;&nbsp; 1) Took 95th percentile for <b> age </b>.

#### Modelling:
Performed KNN, SVM and Decision tree classification on the dataset and compared the results against a baseline model and a simple logistic regression.


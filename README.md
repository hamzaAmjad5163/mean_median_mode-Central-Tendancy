# mean_median_mode-Central-Tendancy
Objective: Apply the concepts of mean, median, and mode to a real dataset to understand the central tendency.
Tasks:
1. Data Preparation:
 Load the dataset into a data analysis tool.
 Ensure data cleanliness and deal with any missing or outlier values.
2. Data Analysis:
 Calculate the mean, median, and mode of the dataset.
 Discuss the implications of each measure of central tendency for this dataset.
 Identify which measure(s) best represent the data and justify your choice.
3. Report:
 Summarize your findings, including any insights gained from the analysis of
central tendencies.
 Discuss any potential biases in the dataset and how they might affect the
measures of central tendency.

4. Reflection:
 Reflect on the importance of understanding the distribution of data through
central tendency measures in data science.

=========================================================================================
import pandas as pd
import numpy as np
# Load the dataset
internet_usage_df = pd.read_csv(&quot;/mnt/data/internet_usage_data.csv&quot;)
# Calculate mean, median, and mode
mean_hours = internet_usage_df['Hours Spent on the Internet'].mean()
median_hours = internet_usage_df['Hours Spent on the Internet'].median()
mode_hours = internet_usage_df['Hours Spent on the Internet'].mode()[0] # mode() returns
a Series, taking the first value
print(f'Mean Hours Spent on the Internet: {mean_hours}')
print(f'Median Hours Spent on the Internet: {median_hours}')
print(f'Mode Hours Spent on the Internet: {mode_hours}')
===========================================================================================


The analysis of the dataset on daily internet usage by individuals has been completed, yielding
the following measures of central tendency:
Mean Hours Spent on the Internet: 4.30 hours
Median Hours Spent on the Internet: 4.55 hours
Mode Hours Spent on the Internet: 3.50 hours
These results indicate that on average, individuals spend around 4.30 hours on the internet
daily. The median value suggests that half of the individuals spend more than 4.55 hours, while
the other half spend less. The mode indicates that the most common daily internet usage
among the individuals in the dataset is 3.50 hours.

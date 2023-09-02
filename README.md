# Data-Science-salary-Prediction


A. Data gathering and integration The first part is to get the data you will use. You may use anything that has not been used in an assignment or tutorial. It must have at least 100 data points and must include both numerical and categorial (or ordinal) variables. I recommend keeping this relatively straightforward because data cleaning can take a lot of time if you choose a large, messy dataset. Kaggle (https://www.kaggle.com/datasets) and the University of California at Irvine (UCI) (https://archive.ics.uci.edu/ml/index.php) maintain collections of datasets, some even telling you if they are good examples for testing specific machine learning techniques. You may also choose to join together more than one dataset, for example to merge data on health outcomes by US state with a dataset on food statistics per state. Merging data is not required and will earn you a bonus point in this step.


Dataset Source : https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023  

Dataset Explaination :

The Data Science Job Salaries Dataset is a collection of information related to salaries in the field of data science. It consists of 11 columns, each providing specific details about the data.

The "work_year" column indicates the year in which the salary was paid, providing a temporal reference for the dataset. The "experience_level" column describes the level of experience the individual had in their job during that particular year. It helps to differentiate between junior, mid-level, and senior positions, or other categories based on experience.

The "employment_type" column specifies the type of employment for the role, such as full-time, part-time, contract, or freelance. This information provides insights into the nature of the job and the terms of employment.

The "job_title" column contains the role that the individual worked in during the year for which the salary information is provided. It helps to identify the specific job titles and positions within the data science field.

The "salary" column represents the total gross salary amount paid to the employee during the specified year. This provides an indication of the financial compensation received by individuals in data science roles.

The "salary_currency" column indicates the currency in which the salary was paid, following the ISO 4217 currency code. This information is crucial for understanding the currency context of the salary data.

The "salaryinusd" column represents the salary amount converted into USD (United States Dollar). This column allows for better comparison and analysis of salaries across different countries or regions.

The "employee_residence" column provides the primary country of residence for the employee during the work year, using the ISO 3166 country code. This information helps to identify the geographical distribution of data science professionals and their corresponding salaries.

The "remote_ratio" column indicates the overall amount of work done remotely by the employee. It provides insights into the remote work culture and practices within the data science industry.

The "company_location" column specifies the country of the employer's main office or contracting branch. It helps to understand the geographical distribution of companies hiring data science professionals.

The "company_size" column represents the median number of people that worked for the company during the year. 

This information provides an understanding of the company's scale and potentially its resources for compensating data science professionals. In summary, this dataset contains comprehensive information about salaries in the data science field, including temporal, experiential, employment, and geographical aspects. It enables analysis and exploration of the factors influencing salaries and their variations across different regions, job titles, experience levels, and company sizes.



B. Data Exploration Using data exploration to understand what is happening is important throughout the pipeline, and is not limited to this step. However, it is important to use some exploration early on to make sure you understand your data. You must at least consider the distributions of each variable and at least some of the relationships between pairs of variables.

Salary Distribution Histogram: This graph shows the distribution of the “salary_in_usd” variable. The x-axis represents the salary values in USD, and the y-axis represents the count of individuals or jobs that fall into each salary range. The “geom_histogram” function is used to create the histogram, with a binwidth of 10,000 USD, meaning the salary range is divided into bins of 10,000 USD each. The bars of the histogram show the frequency or count of salaries falling within each bin.
Salary by Experience Level Boxplot: This graph examines the relationship between “salary_in_usd” and “experience_level”. The x-axis represents the different experience levels, while the y-axis represents the salary in USD. The boxplot displays the distribution of salaries for each experience level. The box represents the interquartile range (IQR), with the line inside the box indicating the median salary. The whiskers extend to the minimum and maximum values, excluding any outliers. Each experience level is represented by a separate boxplot, and the fill color distinguishes between different experience levels.


Salary by Employment Type Boxplot: This graph explores the relationship between “salary_in_usd” and “employment_type”. The x-axis represents the different employment types, while the y-axis represents the salary in USD. The boxplots display the distribution of salaries for each employment type. Similar to the previous graph, the box represents the interquartile range (IQR), the line inside the box represents the median salary, and the whiskers extend to the minimum and maximum values, excluding outliers. Each employment type is represented by a separate boxplot, and the fill color differentiates between different employment types.



















Salary vs. Remote Ratio Scatter Plot: This graph analyzes the relationship between “salary_in_usd” and “remote_ratio”. The x-axis represents the remote ratio (the extent to which a job can be performed remotely), while the y-axis represents the salary in USD. Each data point represents an individual job or person. The geom_point function is used to plot the points, with a purple color. The scatter plot allows us to visualize the distribution of salaries at different levels of remote work. It helps us understand if there is any correlation between the ability to work remotely and the salary level.


















Each graph uses different visualization techniques to represent the relationship or distribution of the “salary_in_usd” variable with other variables. These plots aid in understanding the data and identifying patterns, trends, or insights related to salaries based on different factors such as experience level, employment type, and remote work ratio.

C. Data Cleaning Don’t forget – this can take a lot of the time of the whole process. Your cleaning process                must ensure that there are no missing values and all outliers must be considered. It may be reasonable to just remove rows with missing values, however, if your data or small or that would change the distributions of the variables, that will not be adequate and you will need to consider other options, as discussed in the modules on cleaning. Depending on your data and what you plan to do with it, you may also need to apply other processes we discussed. For example, clean up strings for consistency, deal with date formatting, change variable types between categorical and numeric, bin, smooth, group, aggregate or reshape. Make the case with visualization or by showing resulting summary statistics that your data are clean enough to continue with your analysis.






















In the data cleaning process the dataset is going through cleaning checking for missing values and and removing any outliers and based on output there are no missing values in the code.




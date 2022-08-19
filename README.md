# Summary-Statistics-Challenge-

I've been given access to the complete data from a recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

I was tasked to generate all of the tables and figures needed for the technical report of the clinical study. Also for a top-level summary of the study results.


# Generate Summary Statistics
Create two summary statistics DataFrames:

For the first DataFrame, I used a groupby method to generate the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen. This resulted in five unique Series objects. I combined these objects into a single summary statistics DataFrame.

For the second DataFrame, I used the agg method to produce the same summary statistics table by using a single line of code.


# Create Bar Charts and Pie Charts
I generated two bar charts. Both charts to be identical and show the total number of time points for all mice tested for each drug regimen throughout the study.

- Created a bar chart with the Pandas DataFrame.plot() method.

- Created a second bar chart with Matplotlib's pyplot methods.

- Generated two pie charts. Both charts to be identical and show the distribution of female versus male mice in the study.

- Created a first pie chart with the Pandas DataFrame.plot() method.

- Created a second pie chart with Matplotlib's pyplot methods.


# Calculate Quartiles, Find Outliers, and Create a Box Plot
- Calculated the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. 
    Then, calculated the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. 

With the following substeps:
- Created a grouped DataFrame that shows the last (greatest) time point for each mouse. Merged this grouped DataFrame with the original cleaned DataFrame.

- Created a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

- Looped through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Appended the final tumor volumes for each drug to the empty list.

- Determined the outliers by using the upper and lower bounds, and then print the results.

- Using Matplotlib, I generated a box plot of the final tumor volume for all four treatment regimens. Highlighted any potential outliers in the plot by changing their color and style.


# Create a Line Plot and a Scatter Plot
- Selectd a mouse that was treated with Capomulin, and generated a line plot of tumor volume versus time point for that mouse.

- Generated a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

# Calculate Correlation and Regression
- Calculated the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.

- Plotted the linear regression model on top of the previous scatter plot.

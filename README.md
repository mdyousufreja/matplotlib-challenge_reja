# matplotlib-challenge_reja


What good is data without a good plot to tell the story?

In this assignment, you’ll apply what you've learned about Matplotlib to a real-world situation and dataset.

# Background # 

You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

## Files ##

Downloaded the following files to get started:

Module 5 Challenge [files](https://courses.bootcampspot.com/courses/3819/assignments/56675?module_item_id=999492)


## Instructions ##

This assignment is broken down into the following tasks:

- Prepared the data.

- Generated summary statistics.

- Created bar charts and pie charts.

- Calculated quartiles, find outliers, and create a box plot.

- Created a line plot and a scatter plot.

- Calculated correlation and regression.

- Submitted my final analysis.

### Prepare the Data ###

  1. Ran the provided package dependency and data imports, and then merged the **mouse_metadata** and **study_results** DataFrames into a single DataFrame.

  2. Displayed the number of unique mice IDs in the data, and then checked for any mouse ID with duplicate time points. Displayed the data associated with that mouse ID, and then created a new DataFrame where   
     this data is removed. Used this cleaned DataFrame for the remaining steps.

  3. Displayed the updated number of unique mice IDs.

### Generate Summary Statistics ###

Created a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method I used is less important than the result.

My summary statistics included:

- A row for each drug regimen. These regimen names should be contained in the index column.

- A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

### Create Bar Charts and Pie Charts ###

 1. Generated two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

    - Created the first bar chart with the Pandas **DataFrame.plot()** method.

     - Created the second bar chart with Matplotlib's **pyplot** methods.

 2. Generated two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

     - Created the first pie chart with the Pandas **DataFrame.plot()** method.

     - Created the second pie chart with Matplotlib's **pyplot** methods.

### Calculate Quartiles, Find Outliers, and Create a Box Plot ###

 1. Calculated the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if     
    there are any potential outliers across all four treatment regimens. Use the following substeps:

     - Created a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

     - Created a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

     - Looped through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Appended the resulting final tumor volumes for each drug to the empty list.

     - Determined outliers by using the upper and lower bounds, and then printed the results.

 2. Using Matplotlib, generated a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlighted any potential outliers in the plot by changing their color 
    and style.

**hint**: All four box plots should be within the same figure. Used this [Matplotlib documentation pageLinks](https://matplotlib.org/stable/gallery/statistics/boxplot_demo.html) to an external site. for help   
          with changing the style of the outliers.

### Create a Line Plot and a Scatter Plot ###

1. Selected a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

2. Generated a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

### Calculate Correlation and Regression ###

1. Calculated the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.

2. Plotted the linear regression model on top of the previous scatter plot.

   
### References ###
Data generated by MockarooLinks to an external site., LLC (2022). Realistic Data Generator.

## Introduction

### Profile of Dr. Ignaz Semmelweis
### Background of the problem of childbed fever
### Starting Data Analysis

## Importing Modules: Using pandas for data manipulation and matplotlib for plotting
### Reading Data: Reading yearly data from yearly_deaths_by_clinic.csv using pd.read_csv()
### Displaying Data: Printing the DataFrame to inspect the yearly data
### Alarming Number of Deaths

## Calculating Proportions: Using DataFrame operations to calculate the proportion of deaths (yearly["proportion_deaths"] = yearly["deaths"]/yearly["births"])
### Extracting Data: Filtering DataFrames to separate data for Clinic 1 and Clinic 2 (yearly[yearly["clinic"] == "clinic 1"])
### Displaying Data: Printing the filtered DataFrame for Clinic 1
### Deaths in the Clinics

## Plotting Data: Using matplotlib to plot the yearly proportion of deaths for Clinic 1 and Clinic 2
### The Beginning of Handwashing

## Background on the difference between Clinic 1 and Clinic 2
### Reading Data: Reading monthly data from monthly_deaths.csv using pd.read_csv() with parse_dates parameter
### Calculating Proportions: Calculating the monthly proportion of deaths (monthly["proportion_deaths"] = monthly["deaths"]/monthly["births"])
### Displaying Data: Printing the first rows of the monthly DataFrame
### Effect of Handwashing

## Plotting Data: Using matplotlib to plot the monthly proportion of deaths
### Highlighting the Effect of Handwashing

## Determining Dates: Setting the date when handwashing became mandatory (handwashing_start = pd.to_datetime('1847-06-01'))
### Splitting Data: Dividing the DataFrame into periods before and after handwashing was mandatory
### Plotting Data: Using matplotlib to plot the monthly proportion of deaths before and after the start of handwashing
### More Handwashing, Fewer Deaths?

## Calculating Differences: Calculating the difference in the average monthly proportion of deaths before and after handwashing
### Bootstrap Analysis of Semmelweis' Handwashing Data

## Bootstrap Method: Performing a bootstrap analysis to estimate the reduction in deaths due to handwashing
### Calculating Confidence Interval: Using pd.Series().quantile() to calculate a 95% confidence interval from the bootstrap results
### The Fate of Dr. Semmelweis

## Impact of Semmelweis' findings and rejection by the medical community
### Importance of statistical analysis in supporting scientific findings
### Conclusion: the importance of handwashing for doctors
### This table of contents includes not only the structure of the post but also explains the Python tools and methods used in each section.

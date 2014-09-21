Getting-and-Cleaning-Data-Course-Project
========================================
This is the readme for run_analysis.R.

IMPORTANT! Before running run_analysis, you must be sure the plyr, dplyr, and reshape2 R packages are installed. Without these packages, the script will not function.

NOTE: You should also install the plyr package BEFORE installing the dplyr package; doing so ensures that there are no issues with overlapping or conflicting in regards to those packages

To do this, follow these instructions:

If you're using RStudio,
1. Go to the "Tools" tab on the toolbar at the top of the window.
2. Click "Install Packages"
3. Type the name of the package you want to install in the "Packages" field
4. Hit enter or click the "Install" button
 
If you're using RGui,
1. Go to the "Packages" tab on the toolbar at the top of the window.
2. Click "Install Packages"
3. Choose the region closest to you when asked to select a CRAN mirror.
4. Scroll through the list of packages until you see the one you want, then select it and click "OK", or simply double-click it


run_analysis.R is an R script that ultimately generates a tidy data set from Human Activity Recognition (HAR) data collected from Samsung Galaxy S smartphones. 

First, it downloads and unzips the .zip file containing the data into your default working directory. Then, it extracts the "test" and "train" data sets along with the proper activity label and subject ID data and merges it all into one data frame (titled bigstuff2). 

It then extracts from bigstuff2 only the measurements concerning the mean and standard deviation of each measurement variable, tidies up the column/variable names to be a bit more intuitive, replaces the activity ID numbers with descriptive values (Walking, Sitting, Standing, etc.), and finally returns a tidy data set (titled step5) that contains the average of each variable for each activity and each subject.


Variable Explanations
The column/variable names were tidied up/changed from their original state. What follows is a list of the changes made.
- Empty parentheses and hyphens removed
- "mean" capitalized to "Mean"
- "std" lengthened to "StandardDeviation"
- "Mag" lengthened to "Magnitude"
- t at the beginning of column/variable names lengthened to "Time"
- f at the beginning of column/variable names lengthened to "Frequency"
 
Additionally, variables containing "meanFreq" were retained, although they may not be explicit means of the actual accelerometer/gyroscope data. As explained by the readme from the .zip, meanFreq is the "Weighted average of the frequency components to obtain a mean frequency". I chose to include it within the data set as it technically is a mean of a measurement.




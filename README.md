Getting-and-Cleaning-Data-Course-Project
========================================
This is the readme for run_analysis.R.

IMPORTANT! Before running run_analysis, you must be sure the plyr, dplyr, and reshape2 R packages are installed. Without these packages, the script will not function.

NOTE: You should also install the plyr package BEFORE installing the dplyr package; doing so ensures that there are no issues with overlapping or conflicting in regards to those packages

To do this, follow these instructions:

If you're using RStudio,
- Go to the "Tools" tab on the toolbar at the top of the window.
- Click "Install Packages"
- Type the name of the package you want to install in the "Packages" field
- Hit enter or click the "Install" button
 
If you're using RGui,
- Go to the "Packages" tab on the toolbar at the top of the window.
- Click "Install Packages"
- Choose the region closest to you when asked to select a CRAN mirror.
- Scroll through the list of packages until you see the one you want, then select it and click "OK", or simply double-click it


run_analysis.R is an R script that ultimately generates a tidy data set from Human Activity Recognition (HAR) data collected from Samsung Galaxy S smartphones. 

First, it downloads and unzips the .zip file containing the data into your default working directory. Then, it extracts the "test" and "train" data sets along with the proper activity label and subject ID data into separate data frames and merges it all into one big data frame (titled bigstuff). 

It then extracts from bigstuff2 only the measurements concerning the mean and standard deviation of each measurement variable, tidies up the column/variable names to be a bit more intuitive, replaces the activity ID numbers with descriptive values (Walking, Sitting, Standing, etc.), and finally returns a tidy data set (titled step5) that contains the average of each variable for each activity and each subject.

Credits and Acknowledgements:

Sample Code Book by Kirsten Frank: https://class.coursera.org/getdata-007/forum/thread?thread_id=28

Helped with aggregating a range of columns: http://stackoverflow.com/questions/15651153/why-cant-i-use-aggregate-with-cbind-on-a-range-of-columns-in-a-data-frame

Long Data, Wide Data, and Tidy Data for the Assignment by David Hood: https://class.coursera.org/getdata-007/forum/thread?thread_id=214

Help with using select() from HuangTao: https://class.coursera.org/getdata-007/forum/thread?thread_id=202


Codebook for run_analysis.R

Changes made to variable/column names:
Empty parentheses and hyphens removed
"mean" capitalized to "Mean"
"std" lengthened to "StandardDeviation"
"Mag" lengthened to "Magnitude"
t at the beginning of column/variable names lengthened to "Time"
f at the beginning of column/variable names lengthened to "Frequency"

Additionally, variables containing "meanFreq" were retained, although they may not be explicit means of the actual accelerometer/gyroscope data. As explained by the readme from the .zip, meanFreq is the "Weighted average of the frequency components to obtain a mean frequency". I chose to include it within the data set as it technically is a mean of a measurement.

Variable Explanations
Activity: The activity being performed by the subject. There were 6 recorded activities: walking, walking upstairs, walking downstairs, sitting, standing, and laying.
Subject: ID number denoting the subject performing the activities and gathering data. There are 30 subjects, numbered 1-30.
Time...(X,Y, or Z): denotes time domain signals
Body denotes that




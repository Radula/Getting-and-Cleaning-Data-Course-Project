Codebook for the tidy data set (titled step5 in R)

Changes made to original variable/column names:
- Empty parentheses and hyphens removed
- "mean" capitalized to "Mean"
- "std" lengthened to "StandardDeviation"
- "Mag" lengthened to "Magnitude"
- t at the beginning of column/variable names lengthened to "Time"
- f at the beginning of column/variable names lengthened to "Frequency"
 
Additionally, variables containing "meanFreq" were retained, although they may not be explicit means of the actual accelerometer/gyroscope data. As explained by the readme from the .zip, meanFreq is the "Weighted average of the frequency components to obtain a mean frequency". I chose to include it within the data set as it technically is a mean of a measurement.

Variable Explanations

- As explained in the readme, the values in the data frame are the means and standard deviations of acceleration and angular velocity values, or their frequencies.
- The X, Y, or Z at the end of the variable denote the axis of the movement detected by the accelerometer or gyroscope
- Activity: The activity being performed by the subject. There were 6 possible activities:
  - Walking
  - Walking Upstairs
  - Walking Downstairs
  - Sitting
  - Standing
  - Laying
- Subject: ID number denoting the subject performing the activities and gathering data. There were 30 subjects, numbered 1-30.

- Time and Frequency: At the beginning of the variable title; denote whether the data are time domain signals or frequency domain signals
- Body: Denotes that the acceleration data collected was due to bodily movement/acceleration.
- Gravity: Denotes that the acceleration was due to gravity.
- Acc: Stands for accelerometer; denotes data that was collected by the smartphone's accelerometer.
- Gyro: Stands for gyroscope; denotes data that was collected by the smartphone's gyroscope.
- Jerk: Denotes a "jerk signal" derived from bodily linear acceleration and angular velocity
- Magnitude: Denotes that the data is a measurement of the magnitude of the total 3-dimensional movement signal.
- Mean: Denotes a mean value of the signals collected
- MeanFreq: Mean of the frequency components
- StandardDeviation: Denotes the standard deviation of the signals collected.

Examples: 
- TimeBodyAccMeanX is the mean value of the bodily acceleration signals in the X-axis collected by the accelerometer
- FrequencyBodyGyroMeanFreqZ is the mean frequency of the bodily angular velocity signals in the Z-axis collected by the gyroscope



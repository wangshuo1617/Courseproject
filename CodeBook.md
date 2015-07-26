---
title: "CodeBook"
output: html_document
--- 
In the tidy data set, there are 68 columns and 180 rows. The first two columns indicate which subject do what activities.
And the other 178 columns are the average of data that come from the accelerometer and gyroscope for certain variables.
To get this tidy data set, I merge test set and train set; than take only mean() and std() variables from the merged dataset. After that, I connect the merged dataset with information about subject and activies. Finally, calculate the mean of every variables to get the tidy data set.
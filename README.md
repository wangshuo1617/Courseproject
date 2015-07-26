---
title: "README.md"
output: html_document
---

1. Read test set, train set and feature using read.table(), setting stringsAsFactors = FALSE; than, merge the first two together using rbind().
2. Subset the data set from Step 1. Here, I use the regular experssion to filter variables contains "mean()" and "std()". Base on that, we can get a dataset only has the measurements on the mean and standard deviation for each measurement.
3. Read test label, train label and activities label using read.table();than, merge the first two together using rbind().
4. Use mutate() from "dplyr" package to give activities label data set a descriptive name.
5. Merge the data set form Step 2 and activities label data set. Set descriptive variable names for it.
6. Read subject information using read.table(); than, merge them together using rbind().
7. Merge the subject information data set with the data set from Step 5.
8. Use melt() from "reshape2" package to get a melten data frame from Step 7.
9. Run dcast() from "reshape2" package on the melten data frame from last step to get the tidy data set.
10. Save the tidy data set in a txt using write.table() with row.names = FALSE.
# gettingcreatingdata_finalproject
Coursera Course: Getting and Cleaning Data Final Project

This script uses base R functions and functions from the dplyr package to get a tidy dataset of wearable sensor-gathered data.

For more information: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The data used in this project:  https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 


The script:
Merges the training and the test sets to create one data set.
Extracts only the measurements on the mean and standard deviation for each measurement.
Uses descriptive activity names to name the activities in the data set
Appropriately labels the data set with descriptive variable names.
From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.


==================
How the script works:

1. Loads dplyr package
2. Imports components of test and train datasets
3. Binds components
4. Merges expanded test and train datasets
5. Imports feature names from features.txt file
6. Add feature names to columns
7. Selects only columns with mean and standard deviation measurements
8. Imports activity descriptions
9. Add activity descriptions to table
10. Removes punctuation from column names and expands column names for clarity
11. Groups data by activity and subject
12. Summarizes measurements (mean) by activity and subject
13. Outputs final table as text file

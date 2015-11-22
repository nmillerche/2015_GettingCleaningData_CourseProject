# 2015 Getting and Cleaning Data Course Project
Course Project for "Getting and Cleaning Data" on Coursera (https://class.coursera.org/getdata-034), November 2015.

## Project Description
The purpose of this project is to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. 

One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Here are the data for the project:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Data analysis
-------------

The raw data sets are processed using the included run_analysis.R script to create a tidy data set stored in the file tidy.txt.

### Download data set and store variables

The script first checks to see if the data has been downloaded to the working directory. If it has not, then the script downloads the zip file from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and unzips it within the working directory. Then the script sets directory variables and reads the raw data into tables.

### Merge the training and the test sets to create one data set.

Training data and labels (x_train and y_train) are merged with subject IDs columnwise as train_data. Likewise, test data and labels (x_test and y_test) are merged with subject IDs columnwise as test_data. The data are merged rowwise as merged_data, and column labels applied.

### Extract only the measurements on the mean and standard deviation for each measurement.

Uses the `grepl` function to search the merged data for columns whose labels contain "mean" or "std", as well as the Subject and ActivityId columns. Stores these columns to a subset called "mean_std_data".

### Use descriptive activity names to name the activities in the data set

Takes the activity labels extracted from the "activity_labels.txt" file included with the data set, and replaces the numerical indicators with their corresponding description in the "mean_std_data" ActivityId column.

### Appropriately label the data set with descriptive variable names

Renames the dataset with more descriptive names in CamelCase, rather than abbreviations, to make it easier to read, as follows.
* "Acc" is replaced with "Accelerometer"
* "Gyro" is replaced with "Gyroscope"
* "BodyBody" is replaced with "Body"
* "Mag" is replaced with "Magnitude"
* "t" is replaced with "Time"
* "f" is replaced with "Frequency"
* "tBody" is replaced with "TimeBody"
* "-mean()" is replaced with "Mean"
* "-std()" is replaced with "STD"
* "-freq" is replaced with "Frequency"
* "angle" is replaced with "Angle"
* "gravity" is replaced with "Gravity"

### From the data set in the previous step, create a second, independent tidy data set with the average of each variable for each activity and each subject.

The script creates a tidy data set with the mean for each subject and activity, and ordered by Subject, then ActivityId. This tidy data set is written to the text file "tidy.txt".


## Getting and Cleaning Data

Source dataset https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

## run_analysis.R
This script is for a function with one argument - directory.  The function:
* obtains and unzips the relevant data, and places it in the listed directory
* reduces the data set to represent only the activity and subject ids and the columns with std and mean in the headings
* cleans the data pursuant to best practices (note make.names was NOT used as the lecture information was contradictory to the actions of make.names in the sense that the lecture information indicated periods were not appropriate in column names, and make.names adds periods
* a csv file of the data set is created
* a second dataset of the mean data is created
* csv files are then written to the noted directory and are immediately available for use in analysis

### Instructions for project
*  You should create one R script called run_analysis.R that does the following.
*  Merges the training and the test sets to create one data set.
*  Extracts only the measurements on the mean and standard deviation for each measurement.
*  Uses descriptive activity names to name the activities in the data set
*  Appropriately labels the data set with descriptive activity names.
*  Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## Notes

*  Only variables containing mean() & std() are used.
*  Excluded variables of FreqMean and gravityMean
*  Requires the plyr & reshape2 packages.
*  Assumes the dataset is unzipped in the current working directory.

## Results

* tidydata represents the first dataset - saved as tidydata.csv
* meandata represents the second independent data sets - saved as meandata.csv






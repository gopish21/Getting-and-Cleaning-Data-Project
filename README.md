# Getting and Cleaning Data

## Course Project

You should create one R script called run_analysis.R that does the following.

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive activity names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## Steps to work on this course project

1. Download the data source and uncompress it in ```"./data"``` folder. You'll have a ```UCI HAR Dataset``` folder.
2. Put ```run_analysis.R``` in the parent folder of ```UCI HAR Dataset```, then set it as your working directory using ```setwd()``` function in RStudio.
3. Run ```source("run_analysis.R")```, then it will generate a new file ```tiny_data.txt``` in your working directory.
4. Produce ```CodeBook.md``` with a list of column names (which were taken from ```features.txt```)


## The ```run.analysis.R``` has the following functions: 
1. Load the label codes key from ```activity_labels.txt```.
2. Load the feature key from ```features.txt```.
3. Determine the indices of features containing -mean() or -std()).
4. Load the training and test data sets and only retain data columns determined by indices from step #3.
5. Merge the training and test data sets.
6. Replace label codes in the dataset with text labels determined by step #1.
7. Reshape data to use label and subject as identifiers.
8. Generate the ```tiny_data.txt``` file as the output file.


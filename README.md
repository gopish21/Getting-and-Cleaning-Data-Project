# Getting and Cleaning Data

## Course Project

You should create one R script called run_analysis.R that does the following.

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive activity names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## Steps to work on this course project

1. Download the data source and uncompress it in ```"./data"``` folder. There will be a ```UCI HAR Dataset``` folder in the ```./data``` directory.
2. Place ```run_analysis.R``` file in the ```./data``` folder, then set it as the working directory using ```setwd()``` function in RStudio.
3. Run ```source("run_analysis.R")```, that will generate a new file ```tiny_data.txt``` in the working directory.



## The ```run_analysis.R``` uses the following steps: 
1. Load the label codes key from ```activity_labels.txt```.
2. Load the feature key from ```features.txt```.
3. Load the test data and extract only the measurements on the mean and standard deviation for each measurement.
4. Determine the indices of features containing -mean() or -std()) for training data.
5. Load the training data sets extract only the measurements on the mean and standard deviation for each measurement.
6. Merge the test and training data sets.
7. Generate the ```tiny_data.txt``` file as the output file.


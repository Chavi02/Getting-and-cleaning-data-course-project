#Contents

This repository consists of following files

- CodeBook.md : This markdown document indicates all the variables of the tidy data set.
- README.md : This markdown document explains the transformations involved step by step.
- run_analysis.R : This R script was used to transform the given data to a tidy data set.
- Tidy_Data.txt : This is the tidy data set produced as an output from the R script.

#Running the R script

To run the R script one must have the following files in their working directory
- /train/X_train.txt
- /test/X_test.txt
- features.txt
- /test/y_test.txt
- /train/y_train.txt
- /test/subject_test.txt
- /train/subject_train.txt

**dplyr package must be installed in R for this script to run**

Once you have the unzipped folder as the working directory you can run the given R script which will create a tidy data set in a file named *tidyset.txt*

#Step-wise Transformation 

## Step 1

* Both datasets train and test are loaded in separate dataframes.
* Feature list is loaded which is formatted to good variable names.
* This vector is now used to rename the columns of both data frames

## Step 2
* Merging test and train data set

## Step 3

* Extracts only the measurements on the mean and standard deviation for each measurement.


## Step 4

* Uses descriptive activity names to name the activities in the data set


## Step 5

* dplyr package is used to group merged data frame by subject and activity and written to *Tidy_Data.txt* in the working directory.


# Coursera-Getting-and-Cleaning-Data
Week 4 Course Project - UCI_HAR_Dataset

OVERVIEW

This repository contains the R script and documentation as solutions for the Week 4 Course Project of the 'Getting & Cleaning Data' course.

The purpose of this project is to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis.

A full description of the data used in this project can be found at 'The UCI Machine Learning Repository'(http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

The source data for this project can be found here.(https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)


PROJECT GOAL 

The goal of the project is to create one R script called 'run_analysis.R' that does the following:

        1. Merges the training and the test sets to create one data set.
        
                1.1 Reading files
                        1.1.1 Reading trainings tables
                        1.1.2 Reading testing tables
                        1.1.3 Reading feature vector
                        1.1.4 Reading activity labels
                1.2 Assigning column names
                1.3 Merging all data in one set
        
        2. Extracts only the measurements on the mean and standard deviation 
           for each measurement.
        
                2.1 Reading column names
                2.2 Create vector for defining ID, mean and standard deviation
                2.3 Making necessary subset from setAllInOne
        
        3. Uses descriptive activity names to name the activities in the data 
        set
        
        4. Appropriately labels the data set with descriptive activity names.
        
        5. Creates a second, independent tidy data set with the average of each 
           variable for each activity and each subject.
                5.1 Making second tidy data set
                5.2 Writing second tidy data set in txt file


FILE REFERENCES

'CodeBook.md'
- the reference which contains information on the variables, data set, transformations and work that was done to tidy up the data

'run_analysis.R' 
- the code for the R script used to complete the project goals described

'FinalTidyData.txt'
- the output from the 'runAnalysis.R' R script

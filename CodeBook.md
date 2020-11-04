CODE BOOK 
Getting and Cleaning Data 
Week 4 Course Project
Coursera

This code book refers to the data set that has been summarised and output into the tidy_data.txt file. 

For background information on this data se, refer to the README.md file. 

The structure of the data set is described in the Data section, its variables are listed in the Variables section, and the transformations that were carried out to obtain the data set based on the source data are presented in the Transformations section.

[A] DATA

The following text files were imported and merged.
        
Column names were assigned at the time each file was imported and prior to merge. 
        
Files were imported individually and applicable files were then merged into sets, first all files in the TRAINING set (_train.txt) then all files in the TEST set (_test.txt). 
        
This was done prior to merging the two sets into one larger data set. The features and activity_labels files had column names assigned but were not merged and will be used later.

Text Files Imported:

        'features.txt'
        'activity_labels.txt'
        'subject_train.txt'
        'x_train.txt'
        'y_train.txt'
        'subject_test.txt'
        'x_test.txt'
        'y_test.txt'

The final output data file 'tidy_data.txt' is a text file, containing space-separated values.

The first row contains the names of the variables, which are listed and described in the Variables section, and the following rows contain the values of these variables.


[B] VARIABLES

Each row contains, for a given subject and activity, 79 averaged signal measurements.


[C] IDENTIFIERS

        C1: SUBJECT

        Subject identifier, integer, ranges from 1 to 30.

        C2: ACTIVITY

        Activity identifier, string with 6 possible values:

               1. WALKING: subject was walking 
        
                2. WALKING_UPSTAIRS: subject was walking upstairs
        
                3. WALKING_DOWNSTAIRS: subject was walking downstairs
        
                4. SITTING:subject was sitting
        
                5. STANDING: subject was standing
        
                6. LAYING: subject was laying 


[D] AVERAGE OF MEASUREMENTS

All measurements are floating-point values, normalised and bounded within [-1,1].

Prior to normalisation, acceleration measurements (variables containing Accelerometer) were made in g's (9.81 m.s⁻²) and gyroscope measurements (variables containing Gyroscope) were made in radians per second (rad.s⁻¹).

Magnitudes of three-dimensional signals (variables containing Magnitude) were calculated using the Euclidean norm.

The measurements are classified in two domains:

        Time-domain signals
        (variables prefixed by timeDomain)
        - data from the capture of accelerometer and gyroscope raw signals
        
        Frequency-domain signals
        (variables prefixed by frequencyDomain)
        - data from the application of a Fast Fourier Transform (FFT) to some
        of the time-domain signals


[E] TIME-DOMAIN IN SIGNALS

Average time-domain body acceleration in the X, Y and Z directions:

        timeDomainBodyAccelerometerMeanX
        timeDomainBodyAccelerometerMeanY
        timeDomainBodyAccelerometerMeanZ 
        
Standard deviation of the time-domain body acceleration in the X, Y and Z directions:

        timeDomainBodyAccelerometerStandardDeviationX                 
        timeDomainBodyAccelerometerStandardDeviationY 
        timeDomainBodyAccelerometerStandardDeviationZ

Average time-domain gravity acceleration in the X, Y and Z directions:

        timeDomainGravityAccelerometerMeanX
        timeDomainGravityAccelerometerMeanY
        timeDomainGravityAccelerometerMeanZ
        
Standard deviation of the time-domain gravity acceleration in the X, Y and Z directions:

        timeDomainGravityAccelerometerStandardDeviationX 
        timeDomainGravityAccelerometerStandardDeviationY 
        timeDomainGravityAccelerometerStandardDeviationZ

Average time-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:

        timeDomainBodyAccelerometerJerkMeanX 
        timeDomainBodyAccelerometerJerkMeanY 
        timeDomainBodyAccelerometerJerkMeanZ
        
Standard deviation of the time-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:

        timeDomainBodyAccelerometerJerkStandardDeviationX 
        timeDomainBodyAccelerometerJerkStandardDeviationY 
        timeDomainBodyAccelerometerJerkStandardDeviationZ

Average time-domain body angular velocity in the X, Y and Z directions:

        timeDomainBodyGyroscopeMeanX
        timeDomainBodyGyroscopeMeanY 
        timeDomainBodyGyroscopeMeanZ
        
Standard deviation of the time-domain body angular velocity in the X, Y and Z directions:

        timeDomainBodyGyroscopeStandardDeviationX 
        timeDomainBodyGyroscopeStandardDeviationY 
        timeDomainBodyGyroscopeStandardDeviationZ

Average time-domain body angular velocity jerk (derivation of the angular velocity in time) in the X, Y and Z directions:

        timeDomainBodyGyroscopeJerkMeanX
        timeDomainBodyGyroscopeJerkMeanY
        timeDomainBodyGyroscopeJerkMeanZ

Standard deviation of the time-domain body angular velocity jerk (derivation of the angular velocity in time) in the X, Y and Z directions:

        timeDomainBodyGyroscopeJerkStandardDeviationX                 
        timeDomainBodyGyroscopeJerkStandardDeviationY 
        timeDomainBodyGyroscopeJerkStandardDeviationZ
        
Average and standard deviation of the time-domain magnitude of body acceleration:

        timeDomainBodyAccelerometerMagnitudeMean                 
        timeDomainBodyAccelerometerMagnitudeStandardDeviation

Average and standard deviation of the time-domain magnitude of gravity acceleration:

        timeDomainGravityAccelerometerMagnitudeMean                 
        timeDomainGravityAccelerometerMagnitudeStandardDeviation 
        
Average and standard deviation of the time-domain magnitude of body acceleration jerk (derivation of the acceleration in time):

        timeDomainBodyAccelerometerJerkMagnitudeMean                 
        timeDomainBodyAccelerometerJerkMagnitudeStandardDeviation 

Average and standard deviation of the time-domain magnitude of body angular velocity:

        timeDomainBodyGyroscopeMagnitudeMean                 
        timeDomainBodyGyroscopeMagnitudeStandardDeviation 
        
Average and standard deviation of the time-domain magnitude of body angular velocity jerk (derivation of the angular velocity in time):

        timeDomainBodyGyroscopeJerkMagnitudeMean 
        timeDomainBodyGyroscopeJerkMagnitudeStandardDeviation 


[F] FREQUENCY-DOMAIN IN SIGNALS

Average frequency-domain body acceleration in the X, Y and Z directions:

        frequencyDomainBodyAccelerometerMeanX 
        frequencyDomainBodyAccelerometerMeanY 
        frequencyDomainBodyAccelerometerMeanZ 
        
Standard deviation of the frequency-domain body acceleration in the X, Y and Z directions:

        frequencyDomainBodyAccelerometerStandardDeviationX 
        frequencyDomainBodyAccelerometerStandardDeviationY 
        frequencyDomainBodyAccelerometerStandardDeviationZ 

Weighted average of the frequency components of the frequency-domain body acceleration in the X, Y and Z directions:

        frequencyDomainBodyAccelerometerMeanFrequencyX 
        frequencyDomainBodyAccelerometerMeanFrequencyY 
        frequencyDomainBodyAccelerometerMeanFrequencyZ 
        
Average frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:

        frequencyDomainBodyAccelerometerJerkMeanX 
        frequencyDomainBodyAccelerometerJerkMeanY 
        frequencyDomainBodyAccelerometerJerkMeanZ 
        
Standard deviation of the frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:

        frequencyDomainBodyAccelerometerJerkStandardDeviationX 
        frequencyDomainBodyAccelerometerJerkStandardDeviationY 
        frequencyDomainBodyAccelerometerJerkStandardDeviationZ 
        
Weighted average of the frequency components of the frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:

        frequencyDomainBodyAccelerometerJerkMeanFrequencyX 
        frequencyDomainBodyAccelerometerJerkMeanFrequencyY 
        frequencyDomainBodyAccelerometerJerkMeanFrequencyZ 
        
Average frequency-domain body angular velocity in the X, Y and Z directions:

        frequencyDomainBodyGyroscopeMeanX
        frequencyDomainBodyGyroscopeMeanY 
        frequencyDomainBodyGyroscopeMeanZ 
        
Standard deviation of the frequency-domain body angular velocity in the X, Y and Z directions:

        frequencyDomainBodyGyroscopeStandardDeviationX                 
        frequencyDomainBodyGyroscopeStandardDeviationY 
        frequencyDomainBodyGyroscopeStandardDeviationZ 
        
Weighted average of the frequency components of the frequency-domain body angular velocity in the X, Y and Z directions:

        frequencyDomainBodyGyroscopeMeanFrequencyX                 
        frequencyDomainBodyGyroscopeMeanFrequencyY 
        frequencyDomainBodyGyroscopeMeanFrequencyZ 
        
Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body acceleration:

        frequencyDomainBodyAccelerometerMagnitudeMean 
        frequencyDomainBodyAccelerometerMagnitudeStandardDeviation 
        frequencyDomainBodyAccelerometerMagnitudeMeanFrequency 
        
Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body acceleration jerk (derivation of the acceleration in time):

        frequencyDomainBodyAccelerometerJerkMagnitudeMean 
        frequencyDomainBodyAccelerometerJerkMagnitudeStandardDeviation 
        frequencyDomainBodyAccelerometerJerkMagnitudeMeanFrequency 

Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body angular velocity:

        frequencyDomainBodyGyroscopeMagnitudeMean 
        frequencyDomainBodyGyroscopeMagnitudeStandardDeviation 
        frequencyDomainBodyGyroscopeMagnitudeMeanFrequency 

Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body angular velocity jerk (derivation of the angular velocity in time):

        frequencyDomainBodyGyroscopeJerkMagnitudeMean                 
        frequencyDomainBodyGyroscopeJerkMagnitudeStandardDeviation 
        frequencyDomainBodyGyroscopeJerkMagnitudeMeanFrequency


[G] TRANSFORMATIONS

The data set file source is at https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

The following transformations were applied to the source data:

1) The training and test sets were merged to create one data set.

2) The measurements on the mean and standard deviation (i.e. signals containing the strings mean and std) were extracted for each measurement, and the others were discarded.

3) The activity identifiers (originally coded as integers between 1 and 6) were replaced with descriptive activity names (see Identifiers section).

4) The variable names were replaced with descriptive variable names (e.g. tBodyAcc-mean()-X was expanded to timeDomainBodyAccelerometerMeanX), using the following set of rules: Special characters (i.e. (, ), and -) were removed The initial f and t were expanded to frequencyDomain and timeDomain respectively. Acc, Gyro, Mag, Freq, mean, and std were replaced with Accelerometer, Gyroscope, Magnitude, Frequency, Mean, and StandardDeviation respectively. Replaced (supposedly incorrect as per source's features_info.txt file) BodyBody with Body.

5) The final data set was created with the average of each variable for each activity and each subject.

6) The collection of the source data and the transformations listed above were implemented by the run_analysis.R R script (see README.md file for usage instructions).
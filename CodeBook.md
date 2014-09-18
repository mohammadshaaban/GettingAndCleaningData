This file contains information about the variables, data and transformations used in the project


Data Set Information:

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. 

Check the README.txt file for further details about this dataset.


Attribute Information:

For each record in the dataset it is provided: 
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration. 
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.


The process of cleaning the data follows the below:

1. Merge the training and the test sets to create one data set.
All teh data is present in the files:

- subject_train.txt
- x_train.txt
- y_train.txt

- subject_test.txt
- x_test.txt
- y_test.txt

- features.txt
- activity_labels.txt

Column names were assigned and the data was merged to create one data set

2. Extract only the measurements on the mean and standard deviation for each measurement
A logcal vector was created to containing TRUE values for ID, mean and stdev columns and FALSE values for the others

3. Descriptive activity names were given to name the activities in the data set

4. labeling the data set with descriptive activity names

5. A second, independent tidy data set was created to hold the average of each variable for each activity and each subject

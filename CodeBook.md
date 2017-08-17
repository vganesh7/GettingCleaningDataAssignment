# Getting and Cleaning Data Project

## Data
In this repo, `run_analysis.R` is the script that completes the 5 goals presented in the assignmennt.
1. Merges the training and the test sets to create one data set using the `rbind()` function.
2. Extracts only the measurements on the mean and standard deviation for each measurement using the `grep` function and `features.txt`.
3. Uses descriptive activity names to name the activities in the data set using the `activity_labels.txt`.
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject. This is the `tidy.txt` file.

## Variables
+ These variables were used to store the data from the files: `x_train`, `y_train`, `subject_train`, `x_test`, `y_test`, and `subject_test`
+ These variables were used to merge all the data: `x_data`, `y_data`, and `subject_data`
+ `mean_and_std` is a numeric vector used to extract the desired data.
+ `data_all` merged `x_data`, `y_data`, and `subject_data` into one large dataset
+ `tidy_data` stored the averages which was put into the `tidy.txt` text file.

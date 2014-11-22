#Code Book for Getting and Cleaning Data Course Project

##Source of the original data:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

##Process
The script  run_analysis.R  performs the following process to clean up the data and create tiny data sets:

1. Set path to local folder
2. Read Activity Files from y_test.txt and y_train.txt
3. Read Subject Files from subject_test.txt and subject_train.txt
4. Read Features Files from X_test.txt and X_train.txt
5. Read Labels from activity_labels.txt
6. Merge Data
7. Name variables
8. Merge columns
9. Subset and keep only std and mean
10. Label variables that is easy to understand
11. Creates tidy dataset that requires library(plyr)

##Variables
*testData - table contents of  test/X_test.txt  
*trainData - table contents of  train/X_train.txt  
*data - Measurement data. Combined data set of the two above variables
*testSubject - table contents of  test/subject_test.txt  
*trainSubject - table contents of  test/subject_train.txt  
*subject - Subjects. Combined data set of the two above variables
*labels - table contents of  test/y_test.txt   
*combinedata - Data Labels. Combined data set of the two above variables. 
*featuresNames - table contents of  features.txt  
*features - Names of for data columns derived from featuresNames


##Output
*tidyData.txt
*The first column contains subject IDs.
*The second column contains activity name
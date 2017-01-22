#Data source
* The data for this project: 
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

* The site where the data was obtained: 
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

#The run_analysis.R script performs the following steps to clean the data:
* Read X_train.txt, y_train.txt and subject_train.txt from the “./UCI HAR Dataset/train" folder and store them in train.x, train.y and train.subject variables respectively. 
* Read X_test.txt, y_test.txt and subject_test.txt from the "./UCI HAR Dataset/test" folder and store them in test.x, test.y and test.subject variables respectively. 
* Combine train.x, train.y and train.subject and store it in traindata, combine test.x, test.y and test.subject and store it in testdata, merge traindata and testdata and store it in fulldata. 
* Read the features.txt file from the "./UCI HAR Dataset/" folder and store the data in a variable called featureName. Only extract the measurements on the mean and standard deviation. Get a subset of finalData with the 66 corresponding columns. 
* Clean the column names of the subset. Remove the "()" and "-" symbols in the names, as well as make the first letter of "mean" and "std" a capital letter "M" and "S" respectively. 
* Read the activity_labels.txt file from the "./UCI HAR Dataset/" folder and store the data in a variable called activityName. 
* Clean the activity names in the second column of activityName. We first make all names to lower cases. If the name has an underscore between letters, we remove the underscore and capitalize the letter immediately after the underscore. 
* Properly name the first two columns, "subject" and "activity". The "subject" column contains integers that range from 1 to 30 inclusive; the "activity" column contains 6 kinds of activity names; the last 66 columns contain measurements that range from -1 to 1 exclusive. 
* Finally, generate a second independent tidy data set with the average of each measurement for each activity and each subject. We have 30 unique subjects and 6 unique activities, which result in a 180 combinations of the two. Then, for each combination, we calculate the mean of each measurement with the corresponding combination. So, after initializing the result data frame and performing the two for-loops, we get a 180x68 data frame.
* Write the finalData out to “MergedData.txt" file in current working directory.
* Write the groupData out to “MeanData.txt" file in current working directory.


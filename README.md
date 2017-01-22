# Getting-and-Cleaning-Data
Coursera Getting and Cleaning Data Project


This file explains how run_analysis.R script works.

1. unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

   Make sure the folder “UCI HAR Dataset“ and the run_analysis.R script are both in the current working directory.

2. use source("run_analysis.R") command in RStudio.

3. you will find MeanData.txt (224 Kb) which contains a data frame called groupData in the current working directory

4. use data <- read.table(“MeanData.txt") command in RStudio to read the file. 

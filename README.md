# Getting-and-Cleaning-Data
Coursera Getting and Cleaning Data Project


This file explains how run_analysis.R script works.
First, unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip .
Make sure the folder “UCI HAR Dataset“ and the run_analysis.R script are both in the current working directory.
Second, use source("run_analysis.R") command in RStudio.
Third, you will find two output files are generated in the current working directory:
    MergedData.txt (8.3 Mb): it contains a data frame called finalData.
    MeanData.txt (224 Kb): it contains a data frame called groupData.
Finally, use data <- read.table(“MeanData.txt") command in RStudio to read the file. 

# Getting_and_cleaning_data
This file describes how run_analysis.R script works for the peer_assessment.
1. Unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
2. Make sure the folder "data" and the run_analysis.R script are both in the current working directory.
3. Put the “run_analysis.R" command in RStudio.
4. Two output files are generated in the current working directory:
	◦	merged_data.txt (7.9 Mb): it contains a data frame called cleanedData with 10299*68 dimension.
	◦	data_with_means.txt (220 Kb): it contains a data frame called result with 180*68 dimension.
5.  Use data <- read.table("data_with_means.txt") command in RStudio to read the file. Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features.

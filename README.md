# PythonEvolution

This is the experiment data of the thesis "Python's Evolution on Stack Overflow: An Empirical Analysis of Topic Trends". This dataset is from the open source "Stack Exchange Data Dump", which shares the latest posts information monthly. Our data downloaded for this study was published on September 5, 2023.



## Folder

### Raw Data

This is the raw data of "Stack Exchange Data Dump". We just separate them by year.

## Training Data

Contains two files containing training data for All Posts and Unanswered Posts, respectively. The column 'Grade'  is the result of manual scoring and averaging.

## Predicted Data(xlsx)

Inside is the result of each year after prediction, some of the column names are the original column names in the xml file, some of the column names are added for better prediction of the heat value:

- BodyLength: The length of post content.
- CreateDate: The date calculation is converted to the number of days from column 'CreationDate' to September 30, 2023 (i.e., the last day of the month in which the dataset was published) to avoid the date of some posts being converted to zero.
- ActiveDate: The date calculation is converted to the number of days from column 'LastActivityDate' to September 30, 2023 (i.e., the last day of the month in which the dataset was published) to avoid the date of some posts being converted to zero.
- Score-1: The result of dividing the total number of 'Score' by  the 'CreateDate' (i.e., the value of scores earned per day)

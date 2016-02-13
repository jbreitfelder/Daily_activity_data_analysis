## Daily activity - Readme
## Author : Joanne Breitfelder

Note : This project has been realised in the 
framework of the online specialisation in Data Science 
provided by the Johns Hopkins University (Baltimore),
and available on the Coursera web site. 

## Introduction

It is now possible to collect a large amount of data about personal
movement using activity monitoring devices such as a
[Fitbit](http://www.fitbit.com), [Nike
Fuelband](http://www.nike.com/us/en_us/c/nikeplus-fuelband), or
[Jawbone Up](https://jawbone.com/up). These type of devices are part of
the "quantified self" movement -- a group of enthusiasts who take
measurements about themselves regularly to improve their health, to
find patterns in their behavior, or because they are tech geeks. But
these data remain under-utilized both because the raw data are hard to
obtain and there is a lack of statistical methods and software for
processing and interpreting the data.

This project makes use of data from a personal activity monitoring
device. This device collects data at 5 minute intervals through out the
day. The data consists of two months of data from an anonymous
individual collected during the months of October and November, 2012
and include the number of steps taken in 5 minute intervals each day.

In this repository you will find :

* A detailed report of the whole study : "Daily_activity.md"
* The source file of this report written in R markdown : "Daily_activity.Rmd"
* The .zip and .csv files containing the activity data
* A folder containing the different plots of the report
* An HTML version of the report : "Daily_activity.html"

## Data

The data can be downloaded from the Coursera web site. They are also
available in the present GitHub repository.

* Dataset: [Activity monitoring data](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip) [52K]

The variables included in this dataset are:

* **steps**: Number of steps taking in a 5-minute interval (missing
    values are coded as `NA`)

* **date**: The date on which the measurement was taken in YYYY-MM-DD
    format

* **interval**: Identifier for the 5-minute interval in which
    measurement was taken


The dataset is stored in a comma-separated-value (CSV) file and there
are a total of 17,568 observations.


## Some details about the data analysis...

### Loading and preprocessing the data

We first load the data into R and transform them into a format suitable for the analysis

### Calculation of the mean total number of steps taken per day

We make a histogram of the total number of steps taken each day, ignoring the missing values.
We calculate and report the **mean** and **median** total number of steps taken per day.

### Calculation of the average daily activity pattern

We make a time series plot of the 5-minute interval and the average number of steps taken, averaged across all days. We conclude on the 5-minute interval which contains the maximum number of steps.

### Imputing missing values

There are a number of days/intervals where there are missing values (coded as `NA`). The presence of missing days may introduce bias into some calculations or summaries of the data.

1. We calculate and report the total number of missing values in the dataset (i.e. the total number of rows with `NA`s)

2. We devise a strategy for filling in all of the missing values in the dataset
(we use the mean/median for that day).

3. We create a new dataset that is equal to the original dataset but with the missing data filled in.

4. We make a histogram of the total number of steps taken each day and Calculate and report the **mean** and **median** total number of steps taken per day. 

### Are there differences in activity patterns between weekdays and weekends?

1. We create a new factor variable in the dataset with two levels ("weekday" and "weekend") indicating whether a given date is a weekday or weekend day.

2. We make a panel plot containing a time series plot of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all weekday days or weekend days (y-axis).

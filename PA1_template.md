# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data
The data will be read into a variable named 'data'.

```r
data <- read.csv(unz("activity.zip", 'activity.csv'))
```


## What is mean total number of steps taken per day?
**1. Total number of steps**

```r
total_steps <- sum(data$steps, na.rm = TRUE)
```
The total number of steps per day is 570608.

**2. Histogram of number of steps per day**

```r
hist(data$steps, main = "Histogram of Total Steps per Day", xlab="steps", ylab="frequency")
```

![plot of chunk unnamed-chunk-3](PA1_template_files/figure-html/unnamed-chunk-3.png) 

**3. Mean and median of steps per day**

```r
avg_steps <- mean(data$steps, na.rm = TRUE)
median_steps <- median(data$steps, na.rm = TRUE)
```
- Average steps per day is 37.3826
- Median steps per day is 0

## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?

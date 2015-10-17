# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data

```r
df<-read.csv(unzip("activity.zip"))
```
To calculate the steps per day:

```r
df_steps <- aggregate(. ~ date, df, sum)[,2]
```


## What is mean total number of steps taken per day?

```r
hist(df_steps, xlab = "steps per day")
```

![](PA1_template_files/figure-html/unnamed-chunk-3-1.png) 

```r
mean(df_steps)
```

```
## [1] 10766.19
```

```r
median(df_steps)
```

```
## [1] 10765
```



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?

# Introduction
This is my work from the Google Code-in task Use the simple Cranlogs API to obtain half-yearly R package downloads summaries in 2018.
Below you can see the code with comments.

# Prerequisites
-R
-RStudio
-jsonlite
-curl


# Code Description
The code below can be copied to R and executed as is.

#task4

```
#Use the simple Cranlogs API to obtain half-yearly R package downloads summaries in 2018

library('jsonlite')
stat= jsonlite:: fromJSON("https://cranlogs.r-pkg.org/downloads/total/2018-01-01:2018-12-31")

#The task is to obtain the total downloads of all R packages in 2018, half-yearly and save the results in a single CSV file

library('curl')
write.csv(stat, "C:\\Users\\srish\\Desktop\\stat.csv")

```
# Authors 
-Srishti jain

# Screen recording

![](http://g.recordit.co/cmSlmVxzqO.gif)

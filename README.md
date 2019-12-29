# Introduction
This is my work from the Google Code-in task Use the simple Cranlogs API to obtain R package download summaries in 2018.
Below you can see the code with comments.

# Prerequisites
- R
- RStudio
- jsonlite
- curl


# Code Description
The code below can be copied to R and executed as is.

```
#Use the simple Cranlogs API to obtain R package download summaries in 2018

library('curl')
library('jsonlite')

#The task is to obtain the total downloads of all R packages in 2018 and save the results in a single CSV file.

stat= jsonlite:: fromJSON("https://cranlogs.r-pkg.org/downloads/total/2018-01-01:2018-12-31")

write.csv(stat, "C:\\Users\\srish\\Desktop\\stat.csv")

```

# Screen recording

![](http://g.recordit.co/cmSlmVxzqO.gif)

# Authors 
- Srishti Jain

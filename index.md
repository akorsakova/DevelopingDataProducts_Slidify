---
title       : Choose A Bank Assistant
subtitle    : Application Pitch
author      : Anna Korsakova Bain
job         : Manager - Data Analytics
framework   : RevealJS       # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : default      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---
## Choose a Bank Assistant

Application Pitch

Author: Anna Korsakova Bain

--- .class #id 

## What is the 'Choose a Bank Assistant'?
> * The 'Choose a Bank Assistant' allows users to compare banks by complaints filed to the Consumer Financial Protection Bureau (CFPB) 
<br><br>
> * The public can file complaints with the CFPB for any bank in the United States
<br><br>
> * The 'Choose a Bank Assistant' shows graphical comparisons for all banking related complaints for 2014

--- .class #id 

## What is the CFPB?
> * The CFPB is an independent agency of the United States government responsible for consumer protection in the financial sector
<br><br>
> *  The CFPB writes and enforces rules for financial institutions, examines both bank and non-bank financial institutions, monitors and reports on markets, as well as collects and tracks consumer complaints
<br><br>
> * Additional information on the CFPB can be found on <a href = "http://en.wikipedia.org/wiki/Consumer_Financial_Protection_Bureau"> <font color="FF00CC">Wikipedia</font></a>

--- .class #id 

## How do you choose a bank?
> * Research shows that most people choose a bank based on location convenience, either to the branch or the ATM
<br><br>
> * Not many people take the time to look at how many consumers report issues about their bank. Below is the average monthly number of bank related complaints filed with the CFPB in 2014:
<br><br>



```r
  #Average Number of Complaints for a Given Month in 2014
  round(mean(complaints$totals),0)
```

```
## [1] 1223
```

--- .class #id 

## How will this help me chose a bank?
> * With anywhere between 1,100 and 1,300 complaints a month filed with the CFPB relating to banks, shouldn't we all be doing a little bit more research than the nearest ATM location?


```r
  plot(complaints$months,complaints$totals,type="o",pch=22, lty=2,col="blue",main="CFPB Bank Complaints for 2014", xlab="Month", ylab="Total Number of Complaints")
```

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3-1.png) 

See how your banks stacks up <a href = "https://akorsakovabain.shinyapps.io/ChooseABankAssistant/"> <font color="FF00CC">here                                    </font></a>

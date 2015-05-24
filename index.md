---
title       : Regression Analysis
subtitle    : of mtcars dataset
author      : dds63b
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [quiz, bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- .class #id 

## Introduction

This [Shiny Application](https://dds63b.shinyapps.io/mtcarsApp/) explores correlation and regression analysis of variables in the mtcars dataset available through the ```datasets``` package in R. The user can select 2 variables in a dataset to display a few important relationship data.  

About the dataset:  
The data was extracted from the 1974 Motor Trend US magazine, and comprises fuel consumption and 10 aspects of automobile design and performance for 32 automobiles (1973–74 models). 

--- .class #id 

Column names are:

```r
library(datasets)
names(mtcars)
```

```
##  [1] "mpg"  "cyl"  "disp" "hp"   "drat" "wt"   "qsec" "vs"   "am"   "gear"
## [11] "carb"
```

```r
# For better readability, column names were changed in the Shiny App
```

--- .class #id 

## Usage
The application asks the user to select 2 variables in the dataset and displays:
* boxplot distribution
* t-test analysis of the relationship between both selected variables
* the ¨adjusted R-squared¨ which explains the fit quality between both variables
* residual plots

--- &radio

## Test your knowledge:
A higher adjusted r-squared indicates:

1. _a stronger fit between variables_
2. a weak fit between variables

*** .hint
R-squared is the “percent of variance explained” by the model.

*** .explanation
R is the correlation between the predicted values and the observed values of Y. R square is the square of this coefficient and indicates the percentage of variation explained by your regression line out of the total variation.


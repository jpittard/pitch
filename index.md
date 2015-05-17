---
title       : Regression Calculator
subtitle    : Conveniently modeling your numbers
author      : JPittard
job         : Developing Data Products
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax, quiz, bootstrap] # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

--- &radio

## The Need

Did you ever wish you could run regressions without a bunch of code?

1. _Yes!_
2. Not really

*** .hint 

If you are in this class, probably you want to run regressions...

*** .explanation

The answer is yes. Even a little bit of code is a nuisance compared to having it done for you.

---

## The Solution - Regression Calculator

<a href="https://jpittard.shinyapps.io/shiny/">https://jpittard.shinyapps.io/shiny</a>

On this page, input your comma-separated values, press Submit, and the application will display the following:

Values
  - Slope
  - Intercept
  
Graphs
  - Actual versus fitted values
  - Residuals versus fitted
  - Scale-location
  - Normal Q-Q
  - Residuals vs. Leverage

---


## Code example

Granted, the code isn't that hard...

```r
x <- c(1,2,3,4,5,6,7,8,9,10); y <- c(2,4,5,7,8,12,15,14,16,17)
plot(x, y, xlab = "x", ylab = "y", type = "l"); abline(lm(y~x), col="red")
```

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png) 

. . . but I did need something simple for the exercise.

---

## Root mean square

Here is an example of some math. It doesn't have much to do with pitching my application, but it does show that I am learning!

<p>$$\sqrt{\frac{1}{n}(x^2_1+x^2_2+...+x^2_n)}$$</p>



---
title       : "Developing Data Products"
subtitle    : "Pitch for Course Project"
author      : "Aatish Kumar"
job         : 
framework   : io2012     # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Project in a nutshell

- Visualize several probability distributions
- Understand how they compare with normal distributions
- Developed as a Shiny application
- User can vary:
  - Number of observations
  - Type of distribution
  - Fill and border colors of bars of histogram
- Application output:
  - Histogram of distribution with user selected attributes
  - Descriptive statistics of the chosen distribution
  - Q-Q normal plot of the chosen distribution

--- 
## Normal distribution as an example


```r
# Take 1000 observations and generate summary
data <- rnorm(1000); summary(data)
```

```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##  -2.700  -0.647   0.030   0.040   0.697   3.520
```

```r
# generate histogram and Q-Q plot of the data
par(mfrow=c(1,2)); hist(data); qqnorm(data);qqline(data, col = 2,lwd=2,lty=2)
```

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1.png) 

---
## Shiny application
![Shiny Application](./shiny_app2.png)

---
## Project links
- Links to project:
  - Shiny: [http://aatishk.shinyapps.io/DDP_Course_Project](http://aatishk.shinyapps.io/DDP_Course_Project)
  - Github repo: [http://github.com/aatishk/DDP_Course_Project](https://github.com/aatishk/DDP_Course_Project)
- Links to project pitch:
  - Rpubs: [http://rpubs.com/aatishk/DDP_Course_Project](http://rpubs.com/aatishk/DDP_Course_Project)
  - Github io: [http://aatishk.github.io/DDP_Course_Project](http://aatishk.github.io/DDP_Course_Project)


---
title       : Shiny app for financial calculations
subtitle    : tf
author      : Cvornjek Nejc B.Sc. (Industrial engineering)
job         : Graduate student of industrial engineering and bioinformatics
framework   : html5slides       # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

# Shiny app for financial calculations

---

## Inspiration
- Finance is my passion
- Very inspirational course INTRODUCTION TO FINANCE on COURSERA offered by UNIVERSITY OF MICHIGAN and I highly recommend it to everyone
- The professor Mr. GAUTAM KAUL is AWESOME
- Bring finance closer to people

---

## Introduction

- PV [currency] Present value is a value of how much is some amount of money we expect in future worth today
- FV [currency] Future value is value of how much will be amount of money worth after some time interval
- Loan amortization is process where loan breakdown repayment is done

---

## Mathematical background
Future value could be calculated by equation

$$FV = PV * (1 + r)^n$$

and present value is mathematically expressed

$$PV =\frac{FV}{(1 + r)^n}$$

---

## Examples

Today we put in a bank 1000 dollars and bank gives us 5% interest rate. Calculate the amount of what we will have after 5 years.


```r
FV <- 1000 * (1 + 0.05)^5
FV
```

```
## [1] 1276
```

In the second example calculate how much money do we need today if we want 1000 dollars after 5 years, if we get 5% interest rate.


```r
PV <- 1000 / (1 + 0.05)^5
PV
```

```
## [1] 783.5
```


---
title       : Quebec Students Stats (QSS)
subtitle    : A Comparative Regional Students Population Engine
author      : Francois Belanger
job         : Student, Johns Hopkins/Coursera
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

This suite of applications was created in the context of the "Developing Data Products" course offered by Johns Hopkins University on Coursera. The goal of this exercise is to get familiar with the following tools:

- Shiny: an interactive web framework for R
- Slidify: a presentation tool in R

---

## The QSS application

Using the Shiny package as well as regular R code, the Quebec Students Stats (QSS) application aims to access basic data and summaries for regional many-level students population in the province of Quebec, Canada.

You can try the QSS application and read its complete documentation by click [here](https://frankoboy.shinyapps.io/quebecstudents/).

---

## Data & Results

We used Quebec's Superior Education Department data on projected enrollment for the next semester/year of school in most postsecondary institutions in Quebec. There is a row in the dataset for each Quebec administrative region as well as for totals for the numbers in the other columns, which represent the number of preuniversitary, technical, baccalaureate, master and doctorate students. There is also a row with the sum of those five numbers.

The Results section include the region selected and a table, where each row is a type of students (and the last row for totals) and each results column contains:
- the number of students of that type in that region, 
- the proportion of this type of students in the overall student population of the region, and 
- the proportion of this number of students in the overall student population of that type in all of Quebec.

---

## Example

By selecting Montreal and the three last (university) levels, here are the results QSS would give you.


```
## [1] "Montreal"
```

```
##      Level           Population Region % Quebec Level %
## [1,] "Baccalaureate" "117293"   "59.9"   "65.3"        
## [2,] "Master"        "18152"    "9.3"    "62"          
## [3,] "Doctorate"     "6719"     "3.4"    "66.4"        
## [4,] "Total"         "142164"   "72.6"   "64.9"
```

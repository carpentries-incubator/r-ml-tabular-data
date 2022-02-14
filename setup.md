---
title: Setup
---

## RStudio

Learners should have R and RStudio installed. There are instructions for installing R, RStudio, and additional R packages in the [R Ecology Lesson](https://datacarpentry.org/R-ecology-lesson/#Install_R_and_RStudio).

## R Packages

Please install the following R packages:

- `tidyverse`
- `here`
- `rpart`
- `rpart.plot`
- `randomForest`
- `xgboost`

## Workspace and Data

Create a new RStudio workspace where you will keep all of the files for this workshop. In the project directory (where the `.Rproj` file is), create a subdirectory called `data`. You should then be able to download the data for the workshop using the following commands.

```r
download.file("https://www.openml.org/data/get_csv/49817/wine_quality.arff", 
               here("data", "wine.csv"))
```

{% include links.md %}

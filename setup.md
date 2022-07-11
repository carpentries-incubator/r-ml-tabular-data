---
title: Setup
---

## RStudio

Learners should have **updated versions** of R and RStudio installed. There are instructions for installing R, RStudio, and additional R packages in the [R Ecology Lesson](https://datacarpentry.org/R-ecology-lesson/#Install_R_and_RStudio).

## R Packages

Please install the following R packages:

- `tidyverse`
- `here`
- `rpart`
- `rpart.plot`
- `randomForest`
- `xgboost`

Executing the following line of code in the R console will install all of these packages.

```r
install.packages(c("tidyverse", "here", "rpart", "rpart.plot", "randomForest", "xgboost"))
```

You can view all of the packages installed on your system in the *Packages* tab in RStudio. Alternatively, you can print the names of any missing packages by executing the following command.

```r
setdiff(c("tidyverse", "here", "rpart", "rpart.plot", "randomForest", "xgboost"),
        rownames(installed.packages()))
```

If the above command returns `character(0)`, then you have successfully installed all of the packages that you need for this lesson.

## Project and Data

Create a new RStudio project where you will keep all of the files for this workshop. In the project directory (where the `.Rproj` file is), **create a subdirectory** called `data`. You should then be able to download the data for the workshop using the following commands.

```r
library(here)
download.file("https://www.openml.org/data/get_csv/49817/wine_quality.arff", 
               here("data", "wine.csv"))
```

{% include links.md %}

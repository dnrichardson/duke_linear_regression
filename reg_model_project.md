# Modeling and prediction for movies
Dale Richardson  
`r format(Sys.Date(), "%B %d, %Y")`  

## Setup

### Load packages


```r
library(ggplot2)
```

```
## Warning: package 'ggplot2' was built under R version 3.3.2
```

```r
library(dplyr)
library(statsr)
```

### Load data


```r
load("movies.Rdata")
```

* * *

## Part 1: Data

We have been provided a dataset of 651 **randomly sampled** movies produced and released prior to 2016. 
This dataset contains 32 variables, some of which will not be useful for statistical modeling (i.e. `imdb_url`). We have not been provided any further details as to how the movies were exactly randomly selected, so there may be some unknown bias present in the dataset (unlikely, but possible).

While the movies in this dataset have been selected randomly, it is **not possible to infer causality**. No random assignment into experimental/control groups was conducted regarding these movies. Therefore, we are unable to infer causality and instead can only highlight associations between variables.

* * *

## Part 2: Research question

Should be phrased in a non-causal way (1 pt)
Should be well defined / not vague (1 pt)
Is clear why this is of interest to the author / audience (1 pt)



* * *

## Part 3: Exploratory data analysis

What is the date range for movies in this dataset?
Which variables are collinear? i.e. critics score and audience score?


3 pts for plots
Plots should address the research questions (1 pt)
Plots should be constructed correctly (1 pt)
Plots should be formatted well – size not too large, not too small, etc. (1 pt)
3 pts for summary statistics
Summary statistics should address the research questions (1 pt)
Summary statistics should be calculated correctly (1 pt)
Summary statistics should be formatted well – not taking up pages and pages, etc. (1 pt)
4 pts for narrative
Each plot and/or R output should be accompanied by a narrative (1 pt)
Narrative should interpret the visuals / R output correctly (1 pts)
Narrative should address the research question (2 pts)

* * *

## Part 4: Modeling

Develop a multiple linear regression model to predict a numerical variable in the dataset. The response variable and the explanatory variables can be existing variables in the dataset, or new variables you create based on existing variables.

Specify which variables to consider for the full model (1 pt)
Reasoning for excluding certain variables (2 pts)
Reasoning for choice of model selection method (2 pts)
Carrying out the model selection correctly (5 pts)
Model diagnostics (5 pts)
Interpretation of model coefficients (5 pts)

* * *

## Part 5: Prediction

Pick a movie from 2016 (a new movie that is not in the sample) and do a prediction for this movie using your the model you developed and the predict function in R. Also quantify the uncertainty around this prediction using an appropriate interval.

Correct prediction (2 pts)
Correct quantification of uncertainty around this prediction with a prediction interval (1 pts)
Correct interpretation of prediction interval (1 pt)
Reference(s) for where the data for this movie come from (1 pt)

* * *

## Part 6: Conclusion

A brief summary of your findings from the previous sections without repeating your statements from earlier as well as a discussion of what you have learned about the data and your research question. You should also discuss any shortcomings of your current study (either due to data collection or methodology) and include ideas for possible future research.

Conclusion not repetitive of earlier statements (1 pt)
Cohesive synthesis of findings that appropriate address the research question stated earlier (1 pt)
Discussion of shortcomings (1 pt)

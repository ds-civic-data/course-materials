Homework 1: Visualization
================

### MDSR Exercises

Exercise 2.5, 2.6, 3.3, 3.4, and 3.9

### Exercise 3.11

The `fivethirtyeight` package is a treasure trove of the data that appears in the data journalism articles of [fivethirtyeight.com](http://fivethirtyeight.com/). Select a data set that's interesting to you, create two informative plots, and describe what they reveal. It may be easiest to browse all of the dataset by looking through the [github repository](https://github.com/fivethirtyeight/data) (most but not all of these datasets will be available in the package).

### Exercise 3.12

For this exercise you'll be working with a random sample of the full oregon voter history file. They can be downloaded using the following code:

``` r
library(tidyverse)
vote_particip <- read_csv("http://bit.ly/2l1bIxs")
```

Use this data to craft a visualization that sheds light on a question that you have about htis data. In addition to your visualization, please include some commentary that touches on issues such as:

-   your motivating question
-   what type of variables you're using (e.g. categorical vs. numeric)
-   wht you decided to map those variables to particular visual cues through aesthetics
-   why you used the geometry that you did
-   what additional tweaks you made (if any) to improve the clarity of the graphic (you may want to refer to Tufte's principles)
-   what does this graphic tell you about your motivating question?

### Notes

-   **Data**: The chapter 3 exercises have you constructing your own plots. This should happen in an R chunk in your .Rmd file that begins with loading in the package in which the data is stored. If you're working with the babynames data for instance, you'll want to start your chunk like this:

``` r
library(tidyverse) # loads ggplot2
library(babynames) # load babynames data
data(package = "babynames") # shows which data sets are available
```

-   **Format**: Be sure your .Rmd file has `output: github_document` at the top
-   **Figures**: You can fiddle with the size of the figures that are created in your .Rmd by adjusting what are called the "chunk options". These live inside the curly braces at the top of each R chunk. If you wanted to, for instance, make only very narrow figures, you could open your R chunk with this: \`\`\``{r fig.width = 2}`.
-   **Files**: You'll notice that once you start knitting a .Rmd with plots, if you have set your output to `github_document`, you'll start seeing extra files pop up in your git pane. These are the figures that will get placed into your .md file on github, so be sure to commit and push these as well.

Homework 4: Import
================

### Overview

To gain experience with the process of Data Import (with all its peculiarities) please do the following:

1.  Find **two** data sets of a novel kind, and **one** that is specifically civic data
2.  Import them into R
3.  Tidy them, if needed
4.  Transform them, if needed
5.  Visualize the data and provide a short interpretation of the what the graphic tells you

The .Rmd file that you compose for this assignment should have a section for each data set and subsection for each of the following: Import, Tidy, Transform, Visualize.

### Finding the data

The two sets that you will be working with should be of a type that you have never before brought into R. This is to get your outside of the lingua franca flat tiles that you're been reading in using the `readr` package (e.g. `read_csv()`). As a reminder, these could be:

**Proprietary flat files**

-   STATA
-   SPSS
-   Minitab
-   Octave/Matlab
-   Excel
-   GoogleSheets

**Relational Database**

-   MySQL
-   SQLite
-   Postgres

**Hierarchical Data**

-   JSON
-   XML
-   (HTML)

To start you in your hunt for data, you can explore the following links:

-   The ICPSR is the world's largest repository of social, behavioral, and economic data. [icpsr.umich.edu](http://www.icpsr.umich.edu)
-   Data.gov is the home of the U.S. government's open data. There is more information there than anyone can possibly absorb! [data.gov](https://www.data.gov/)
-   The Roper Center houses more than 50 years of public opinion data on a wide variety of political and social issues. There are surveys conducted in the 1930s! [ropercenter.uconn.edu](https://ropercenter.cornell.edu/)
-   Care about world development? The go to source for information on economic and social development indicators is the World Bank's data repository, [data.worldbank.org](https://data.worldbank.org/)
-   One of the most exciting developments in data dissemination is the "Dataverse", a project started at Harvard University, but which has spread worldwide. Anyone can have a dataverse, and there are more than 2000 that you can browse. [dataverse.org](https://dataverse.org/)

You're also welcome to find your own data, just be sure this is the first time you've read that type of data into R. There are many, many more options for you to investigate, public and private, governmental and non-governmental. Good hunting!

You might come across data that is not immediately available for download, but is instead available only through an application programming interface or API. An API is a set of protocols that you can use efficiently interact with a large database over the web. If you find data that's available via API, we encourage you to explore it - some of the most interesting data out there will be of this class (including Twitter data).

### Import into R

-   Once you find a data set, you might be able to read it directly into R by providing the url (e.g. `read_csv("bit.ly/SEOj2")`) but most likely you will need to
    -   download it to your computer
    -   upload it to RStudio
    -   read it in by providing it the correct path
-   If you are uploading data to the RStudio server, please create a `/data` folder in your `homework` folder and drop the data set there. If your data set is small (&lt; 10 megs), it should be find to commit send to GitHub.
-   If the data set is large, **do not commit the data set**. GitHub will chocke if you try to push a large data set. The best strategy is to open up the `.gitignore` file in RStudio and add a line of text that says `homework/data/`. If you keep your eye on the Git pane in the upper-right corner as you save this file, you should see all those data files disappear - they will no longer be tracked by Git. You can still compute with the data set in RStudio, make your homework Rmd file, and commit that to send off the GitHub.
-   Another useful tactic when computing with large data sets is to cache the output of your R chunks using the `cache = TRUE` option. Similar to the data, please **do not commit the cache folder**, just add it to your `.gitignore`.
-   You will almost certainly need to download and install a new package to read in your two new data sets. To find the right package, start off by googling around. If you still can't figure it out, ask on slack.

------------------------------------------------------------------------

### Civic Data

Here we'll define civic data as a data set collected at the neighborhood (Woodstock), city (Portland), county (Multnomah), or state (Oregon) level that somehow informs public life. This will likely be data collected by the government, but it might come from the more general community. You are welcome to find this data anywhere, but here are some good spots to start:

-   [State of Oregon Open Data](https://data.oregon.gov/)
-   [City of Portland Bureaus](https://www.portlandoregon.gov/26003)
-   [Portland Civic Apps](http://civicapps.org/datasets/)
-   [Portland Spatial Data](http://gis-pdx.opendata.arcgis.com/)

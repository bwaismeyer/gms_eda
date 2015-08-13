# Exploratory data analysis of gun violence and gun sales.

### Key Questions
1. How do US gun sales behave following mass shootings in the US?
  * H1: Gun sales spike in the short-term following mass shootings.

### Needs
* gun sale data (Google database?)
  * date (as micro as possible, week probably the maximum length we want to work with), 
  * location (ideally micro, but aiming for at least state level)
* mass shooting data (look for website or repo)
  * date (day/month/year), 
  * location (ideally micro, but aiming for at least state level)
* location political data (look for website or repo)
  * some rating of political affiliation for the locations of interset (ideally micro, but aiming for at least state level)

### EDA Visualization
* sale trends
  * sales over time (line)
  * sales by location (map)
  * sale by location over time (line and/or fancy map)
* mass shooting trends (geom_line)
  * shootings over time
  * shootings by location
  * shootings by location over time
* political trends
  * ratings over time
  * ratings by location
  * ratings by location over time
* key combinations of the above
  * overlay of shootings and sales over time (line)
    * same but by location (line and/or fancy map)
    * same but by political rating (line)

### Analyses
* time series analysis - ARIMA forecasting and/or odds-for-time-chunks (survival)
* hlm approach (paul details incoming!)

### Milestones
* identify data sources and strategize for how to extract needed data (Wed, Aug 26)
  * gun sales data: Paul
  * mass shooting data: Brian
  * NEXT MEETING: review Roxygen and package styling, review R Markdown, plan implementation of data gathering/cleaning

### Technical Requirements
* work should be done in R and documented for integration into an R package Roxygen-style
* work needs to be documented such that it can be easily shared via blogs
* SHOULD NOT BE IN PIG LATIN EVER, PAUL

# Exploratory data analysis of gun violence and gun sales.

### Key Questions
1. How do US gun sales behave following mass shootings in the US?
  * H1: Gun sales spike in the short-term following mass shootings.

### Data Targets
* gun sale data (Google database?)
  * date (as micro as possible, week probably the maximum length we want to work with), 
  * location (ideally micro, but aiming for at least state level)
* mass shooting data (look for website or repo)
  * date (day/month/year), 
  * location (ideally micro, but aiming for at least state level)
* location political data (look for website or repo)
  * some rating of political affiliation for the locations of interset (ideally micro, but aiming for at least state level)

* some secondary bits that might be nice to know
 * total rates of violence/homicide and total rates involving a gun (to put frequency of mass violence in context) - scale to match whatever time period we assess (e.g., make both annual or get totals over the window of interest)

### Data Sources
#### mass shootings
* [Mother Jones](http://www.motherjones.com/politics/2012/12/mass-shootings-mother-jones-full-data) is presented as a complete data set of US mass shootings from 1982-2015 (multiple formats, static links available)
 * 72 cases
 * includes date (day/month/year), location (city/state), weapon, and summaries of several other shooting details
 * method details are scattered across several pieces: 
  * the dataset itself lists sources/methods for how each case was identified and verified
  * [Mother Jones report using the data, including explicit criteria discussion](http://www.motherjones.com/politics/2012/07/mass-shootings-map)
  * [argument by some scholars using the Mother Jones data that shootings are increasing in frequency](http://www.motherjones.com/politics/2014/10/mass-shootings-rising-harvard)
  * [more focused article on the authors' analysis/methods, including some chatter about the Mother Jones data](http://www.motherjones.com/politics/2014/10/mass-shootings-increasing-harvard-research)
 * only counts shootings with 4+ deaths (not including the suspect, FBI definition)
 * should get at least one other data source to compare this against (for instance, [this report](http://www.gannett-cdn.com/GDContent/mass-killings/index.html#frequency) suggests the dataset may be incomplete - should review the dataset logic more carefully to see what the inclusion/exclusion criteria and methods are exactly
* [USA today report](http://www.gannett-cdn.com/GDContent/mass-killings/index.html#explore) is completed as complete set of US massing "killings" from 2006-2015 (no obvious sharing format - likely needs to be scraped)
 * 287 cases
 * includes date (day/month/year), location (place/state), method, type, victims, and more
 * method details found [here](http://www.gannett-cdn.com/GDContent/mass-killings/index.html#title) by clicking on the "i", also only 4+ deaths
 * intentional effort to address errors and missing events in FBI records
 * includes more than gun mass killings
* [this report](http://archive.is/f4gbv) claims a 227 incidents in a very short window of time - 2009-2013 - but may have a broader definition of shooting which it calls "rampage shooting"
 * lacks incident-level data and will need to dig to understand methods or assess credibility, but may be useful to contrast against other data sources and to assess rate of shooting "sprees" that don't fit 4+ criteria
* [Stanford Library](https://library.stanford.edu/projects/mass-shootings-america/data) database for US mass shootings from 1966 to ?
 * total cases not stated but seems like a very formally structured/maintained dataset - however visible visualizations do not seem that densely populated...?
 * need to request data access but an online process in place
* [FBI summary and maybe data](https://www.fbi.gov/news/stories/2014/september/fbi-releases-study-on-active-shooter-incidents/pdfs/a-study-of-active-shooter-incidents-in-the-u.s.-between-2000-and-2013) for 2000-2013
 * 160 cases
 * it's in a pdf...? yup...
 * may be well covered by the USA today data but has useful summaries and definitions beyond the data itself
* [more recent Congressional Research report](http://reason.com/blog/2015/08/03/mass-shootings-study) for 1999-2013 and also references to an independent study for 1970+...
 * need to dig to see if there's actually any data available and what it involves... but has useful breakdowns and totals to contrast against other avaialable data sources but seems an excellent review of the key concepts around mass shootings v. other events and an excellent summary of key data sources...
 * NOTE: first attempt to locate one of the data sources failed - may have been removed from site it was on

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

---
title       : Exploring Working Hours  
subtitle    : per Week per Country from 1980 - 2007 
author      : Fernando Hernandez
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Data Used

Data courtesy of Gapminder / International Labour Organization

- Direct download at 
1.  http://spreadsheets.google.com/pub?key=rdCufG2vozTpKw7TBGbyoWw&output=xls

- Gapminder Data
2.  http://www.gapminder.org/data/

- Link to complete reference  
3.  http://www.ilo.org/public/english/employment/strat/kilm/download.htm

--- .class #id 

## Overview  

**Currently running at** https://fernando.shinyapps.io/WorkingHours/  

  
  
This app is intended to allow the user to explore the csv data that is publicly available.
- The linked csv is directly loaded and all processing is done server-side starting with the original csv file.

Hours per week are defined as
- Total amount of yearly working hours divided by 52 weeks.

The user can customize time series plots, boxplots, summary data, and a breakdown by decade.


--- .class #id

## Time Series Graph



Customization includes

- Selecting the countries to plot.

- Custom quantile bars of distributions of means for all all countries each year. 
(defaulted at middle 50% of the data)

- Values for each country (or median of all countries) can be added to the graph.
- Values are also stored in the Summary tab.

- Min/Max bars can be added which show the entire range of the means of each year for all countries.

- All graphs have the option to include a custom theme courtesy of the ggthemes package.

--- .class #id


## Summary Page

- All values from world statistics and for each country which is selected are dynamically loaded here.

- Countries can be added or removed within this tab as well

- Currently it may take a bit of switching between tabs at first to generate initial Summary data.

- Blank values in country summaries represent NA values where no data was reported for that particular year and country.

--- .class #id

## Boxplots and Decades Graph

- Countries may be added to Boxplots.

- Custom themes can be added to either.

- Full Source Code is available at  


1. https://github.com/FCH808/GapminderHoursWorked
  * Bugs or revisions may be submitted here



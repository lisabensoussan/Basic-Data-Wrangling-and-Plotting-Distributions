# Democracy Index Analysis - Lab 1: Basic Data Wrangling and Plotting, Distributions

## Project Overview

This project provides an in-depth analysis of the World Democracy Index dataset. It utilizes data manipulation techniques and statistical visualization methods in R to explore global democracy trends over time, specifically focusing on the years 2006 to 2022.

## Objectives

- Load and process the Democracy Index data from various sources.
- Conduct comparative analyses of countries based on their democracy scores.
- Visualize global trends in democracy over time, including regional and country-specific patterns.
- Assess the impact of democracy index changes on socio-economic variables such as GDP, population, and incarceration rates.
- Estimate regime transition probabilities and display them via heatmaps.
- Display global data on a world map for visual analysis.

## Key Features

Data Sources
- Democracy Index: Data scraped from Wikipedia's Democracy Index page and processed into meaningful insights.
- Additional Data: GDP (PPP) per capita, population size, incarceration rates, and land area data were also incorporated for further analysis.

## Analysis and Visualizations

1. World Democracy Index Dataset:
   - Analysis of the top and bottom countries based on democracy index scores in 2022.
   - Comparative analysis of regional democracy index distributions.

2. Plotting Distributions:
   - Boxplots and density plots were created to explore the distribution of democracy scores by region.
   - Outliers were identified, and statistical summaries such as mean, variance, skewness, and kurtosis were calculated.

3. Country Comparisons & Trends:
   - Developed a custom R function to compare democracy index changes across countries and regions over time.
   - Grouped countries based on significant changes in democracy index between 2006 and 2022.

4. Regime Transitions:
   - Estimated the empirical probabilities of regime transitions (e.g., Full democracy to Authoritarian) between 2006 and 2022.
   - Displayed results via a heatmap for easy interpretation.

5. Additional Data Integration:
   - Integrated data on GDP per capita, population size, incarceration rates, and land area to explore relationships with democracy.
   - Performed regression analysis to assess the impact of democracy index on GDP and incarceration rates.

6. Cumulative Distribution Functions (CDFs):
   - Created CDFs to explore the distribution of GDP per capita, considering random country selection, population size, and land area.

7. World Map Visualizations:
   - Visualized the global democracy index on a world map, displaying both average scores and changes between 2006 and 2022.

8. Democracy Index Components:
   - Analyzed the five components of the Democracy Index (Electoral process, Functioning of government, Political participation, Political culture, Civil liberties).
   - Displayed a heatmap of the correlation between these components and ran a multiple regression analysis to predict GDP per capita.


## Prerequisites

The following libraries are required to run this analysis:
```r
library(tidyverse)
library(data.table)
library(rworldmap)
library(ggthemes)
library(reshape2)
library(e1071)
library(rvest)
library(corrplot)
library(moments)
library(spatstat.geom)

```

## Instructions

1. Run the RMarkdown (Rmd) File:
   - This file contains all the analysis code, figures, and textual explanations.
   - Ensure all the necessary libraries are installed before running the script.

2. Output:
   - The final output should be an HTML file, which can be generated by knitting the Rmd file.

## Results

The top five countries with the highest democracy scores in 2022 are: Norway, New Zealand, Iceland, Sweden, Finland.
The bottom five countries in 2022 are: Afghanistan, Myanmar, North Korea, Central African Republic, Syria.
Detailed country trends and regime change probabilities were calculated and displayed.

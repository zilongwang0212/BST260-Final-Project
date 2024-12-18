
# State-Level and Country-Level Analysis of

# COVID-19 in the United States

## Project Overview

This project analyzes COVID-19 cases and deaths across states in the
United States

using publicly available data from the CDC and population data from the
U.S. Census

Bureau. It includes data cleaning, integration, and visualization to
identify trends

and death rates over four defined pandemic waves.

## Dependencies

### Software

R (version ≥ 4.0)

RStudio (recommended)

### R Packages

Ensure the following R packages are installed:

```{r}
library(readxl)
library(stringr)
library(lubridate)
library(ggplot2)
library(tidyverse)
library(patchwork)
library(httr2)
library(gridExtra)
```

## Data Sources

### COVID-19 Cases

Source: CDC COVID-19 Cases API Endpoint:
<https://data.cdc.gov/resource/pwn4-m3yp.json>

### COVID-19 Deaths

Source: CDC COVID-19 Deaths API Endpoint:
<https://data.cdc.gov/resource/r8kw-7aab.json>

### Population Data

Source: U.S. Census Bureau File: NST-EST2023-POP.xlsx Location: Place
this file in the data/raw-data folder.

## Folder Structure

``` plaintext
BST260-Final-Project/
|
├── code/
|   └── code.qmd    # The code script for wrangling and analysis 
|   └── final-project.qmd    # The script can be rendered to produce the final report
|   └── supplementary-methods.qmd    # The script can be rendered to produce the separate Supplementary Methods
|   └── code.pdf   
|   └── final-project.pdf   
|   └── supplementary-methods.pdf    
|
├── data/
|   └── raw-data/
|       └── NST-EST2023-POP.xlsx    # The population data can be used to calculate the rates
|
├── docs/
|   └── code.pdf   
|   └── final-project.pdf   
|   └── supplementary-methods.pdf    
|
└── README.md                   # Current file
```

## How to Run the Project

### Step 1: Install Required Packages

```{r}
install.packages(c("tidyverse", "ggplot2", "lubridate", "patchwork", 
                   "httr", "stringr", "readxl", "gridExtra"))

```

### Step 2: Run the Supplementary

Open the code.qmd file in `code` directory. And then render the file to
get the code we used in this project.

### Step 3: Final Project

Open the final-project.qmd file in `code` directory. And then render the
file to get the report.

### Step 4: Run the Supplementary

Open the supplementary-methods.qmd file in `code` directory. And then
render the file to get the supplementary methods.

<!-- PROJECT LOGO -->
<br />
<div align="center">
    <img src="images/btg_logo.png" alt="Logo" width="140" height="140">
  </a>
  </div>
  
# Black Thrive Shared Measurement System Methodology
 
## Overview

This Rproject contains the scripts and data necessary to produce the methodology paper supporting Black Thrive's Shared Measurement System for Lambeth, Haringey, and Birmingham. It outlines in detail the data processing and analysis procedures and results that yield each of the Shared Measurement Systems. 

The aim of the Shared Measurement System project is to quantify racial inequality in Britain by comparing various indicators for the Black population with the White population. Doing so makes it possible to identify the aspects of life in Britain where inequality is manifest and to highlight where change is needed.

## Requirements

### Programs

RStudio is required to open and run these scripts. This project was produced using 

- RStudio 2021.09.0 Build 351 "Ghost Orchid"
- R version 4.1.1

### Packages required

The scripts use the following R packages. These need to be installed using <b>install.packages("</b>package name<b>")</b> if they are not already installed on your system.

- gmodels
- tidyverse
- ggrepel
- kableExtra
- epitools
- scales
- showtext
- jsonify
- leaflet
- mapview
- httr

## Contents

**sms_methodology.Rproj**: Project file.

### Data

**data/Stops_LDS_Extract_12MonthsToEnd_202109.zip**: Stop and Search data for Lambeth. csv file within needs to be unzipped to data folder

**data/lambeth_cla_2019.csv**: Data for Children Looked After indicator

**data/lambeth_employment_rate_march_2021_v2.csv**: Employment rate data

**data/lambeth_gcse_2019_2020.csv**: Data for number of pupils achieving at least Level 4 in GCSE English and Maths

**data/lambeth_gld_2018_2019.csv**: Data for number of children reaching a Good Level of Development at age 5.

**data/lambeth_population.csv**: Data for population estimates

**data/lambeth_stat_homeless_jun_2021.csv**: Data for number of households statutorily homeless or at risk of becoming homeless

**data/haringey_stop_search_2020_2021_v2.csv**: Stop and Search data for Haringey

**data/haringey_children_looked_after_2018_2019_v3.csv**: Data for Children Looked After indicator

**data/haringey_employment_rate_2020_2021_v3.csv**: Employment rate data

**data/haringey_4_plus_gcse_english_maths_2019_2020_v2.csv**: Data for number of pupils achieving at least Level 4 in GCSE English and Maths

**data/haringey_good_development_2018_2019_v2.csv**: Data for number of children reaching a Good Level of Development at age 5

**data/haringey_stat_homeless_2020_2021_v2.csv**: Data for number of households statutorily homeless or at risk of becoming homeless

**birm_geo.json**: File containing the longitude and latitude coordinates specifying the boundary of Birmingham.

**data/birmingham_stop_search_2020_09_2021_08.csv**: Stop and Search data for birmingham.

**data/birmingham_cla_2018_2019_v2.csv**: Data for Children Looked After indicator

**data/birmingham_employment_rate_2020_2021_v2.csv**: Employment rate data

**data/birmingham_4_plus_gcse_english_maths_2019_2020_v2.csv**: Data for number of pupils achieving at least Level 4 in GCSE English and Maths

**data/birmingham_good_development_2018_2019_v2.csv**: Data for number of children reaching a Good Level of Development at age 5

**data/birmingham_stat_homeless_2020_2021_v2.csv**: Data for number of households statutorily homeless or at risk of becoming homeless

### Scripts

**scripts/methodology.Rmd**: Script for processing and analysing data and presenting results

**scripts/methodology.html**: Knitted html markdown file generated by above script

**scripts/ors_rrs.bib**: Bibtex file for bibliography

**scripts/style.css**: Formatting file for text

### Other

**images/btg_logo.png**: Black Thrive logo

**images/map.png**: Birmingham area map defined by coordinates used for Birmingham Stop and Search query

## Setup

Once downloaded, unzip to a destination of your choice. Note that the Stop and Search data for Lambeth also needs to be unzipped, with the resulting csv file being located in the ***data*** directory. Be sure to retain the original folder structure.

Use **sms_methodology.Rproj** to open project. 

To load the main script, use *File > Open File*, navigate to the ***scripts*** folder, and select **methodology.Rmd**. To run the script, select *Run > Run all* (Ctrl + Alt + R [Windows]; Cmd + Option + R[Mac]).

If you just want to view the knitted html document, using your system file navigator navigate to the scripts folder and open **methodology.html** in your preferred browser.

## Contact

If you have any questions, comments, or feedback please contact the Research Team at Black Thrive: research@blackthrive.org, FAO Jolyon Miles-Wilson.
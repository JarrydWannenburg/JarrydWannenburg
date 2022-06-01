# Introduction (NOTE: Portfolio is currently under construction)
Hi! I'm Jarryd. I recently graduated from the University of Georgia (2018-2022) with a certificate in Financial Technologies, a BBA in Management Information Systems (MIS) with an emphasis in Data Analytics, and a MS in Business Analytics. Starting September 2022, I'll be working with EY as a Financial Services Technology Consultant. 

## Personal Goal
Within the next 5 years (2027), I want to have built a comprehensive portfolio of projects, completed my MBA, and be leading teams focused on driving decisions using data! Wish me luck!

# Portfolio Directory
A repository consisting of work completed through part-time work, personal projects, and online courses. These projects will primarily be in R and Python though visualization may be done using Tableau, Data Studio, or PowerBI.
* [Data Analytics](https://github.com/JarrydWannenburg#data-analytics)
    * [Google Data Analytics Capstone 1](https://github.com/JarrydWannenburg#google-data-analytics-capstone-1)
* [Data Science](https://github.com/JarrydWannenburg#data-science)
    * [Doggy Shoes](https://github.com/JarrydWannenburg#Doggy-Shoes)
* [Web Application Development](https://github.com/JarrydWannenburg#web-application-development)
    * [LightingCalc](https://github.com/JarrydWannenburg#lightingcalc)
    * [SupplementalCalc](https://github.com/JarrydWannenburg#supplementalcalc)
    * [TargetCalc](https://github.com/JarrydWannenburg#targetcalc)
    * [SolarPanelEstimator_one](https://github.com/JarrydWannenburg/JarrydWannenburg/blob/main/README.md#solarpanelestimator_one)
    * [SolarPanelEstimator_multi](https://github.com/JarrydWannenburg/JarrydWannenburg/blob/main/README.md#solarpanelestimator_multi)

## Data Analytics
### Google Data Analytics Capstone 1 (in progress)
[![](https://img.shields.io/badge/GitHub-Read_Report-4285F4?logo=GitHub)](https://github.com/JarrydWannenburg/Divvy-Trip-Data-Google-Analytics-Capstone/blob/main/Report.md)
[![](https://img.shields.io/badge/GitHub-View_on_GitHub-6e5494?logo=GitHub)](https://github.com/JarrydWannenburg/Divvy-Trip-Data-Google-Analytics-Capstone)
[![](https://img.shields.io/badge/YouTube-Watch_Presentation-FF0000?logo=YouTube)]()

**Concepts:** Data Analytics, Data Visualization, Data Transformation

**Skills:** R (tidyr, dyplr, ggplot2, lubridate), Tableau, Powerpoint

**Description:** In this case study, I used bike sharing data spanning the last 12 months in Chicago to analyze and differentiate two user plans. I was then able to develop a series of visuals and recommendations based on those findings.


## Data Science
### Doggy Shoes
[![](https://img.shields.io/badge/GitHub-View_on_GitHub-6e5494?logo=GitHub)](https://github.com/JarrydWannenburg/Doggy-Shoes)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tRaS8DhK9yJH3oqBQzw87_NnFeKsWz4h?usp=sharing)

**Concepts:** Machine Learning, Linear Regression

**Skills:** Python (pandas, statsmodels)

**Description:**
Build a machine learning model (using OLS) to estimate doggy shoe size from a given harness size and other features.

## Web Application Development
During my time in grad school (August 2021 - May 2022), I held a part-time solo developer position with the MIS department at the Terry School of Business and built out several web applications which are accessible below.

These web applications were developed for greenhouse growers as part of [Project LAMP](https://www.hortlamp.org/outreach/determine-lighting/), lighting approaches to maximize profits. Our goal is to maximize controlled environment agriculture (CEA) grower profits through improved lighting systems and support tools.

These calculators (LightingCalc, SupplementalCalc, and TargetCalc) use a geolocation API to transform a user inputted zipcode to latitude and longitude which is then passed to the TMY API to retrieve location specific weather data. The core idea behind the calculators is this: plants require light to grow. There's an optimal (target) amount of light that a plant can receive over the course of the day (Target DLI). These calculators all focus on the target DLI, but they do so in different ways.

To use this web-based tool, you can add a location anywhere in the US and provide your electricity rate at that location ($/kWh). Add the daily light integral (DLI) you want to achieve and a greenhouse design to get estimated electricity cost results:

### LightingCalc
[![](https://img.shields.io/badge/ShinyApps.io-Open_Web_App-3686d3?logo=r)](https://3dcxni-jarryd-wannenburg.shinyapps.io/LightingCalc/)
[![](https://img.shields.io/badge/GitHub-View_on_GitHub-6e5494?logo=GitHub)](https://github.com/JarrydWannenburg/LightingCalc)
[![](https://img.shields.io/badge/YouTube-Watch_User_Walkthrough-FF0000?logo=YouTube)](https://youtu.be/eSmopYUls30)

**Concepts:** APIs, Data Transformation, Data Analytics, Data Visualization, Web App Development

**Skills:** R (shiny, dyplr, ggplot2, lubridate, tidygeocoder)

**Background:** When I started my assistantship,the two previous students who held this position and graduated over the last two years had developed LightingCalc. My first task was to tweak the UI and server code to display values at a weekly view as opposed to a monthly view and add in demand charges. After familiarizing myself with LightingCalc, I discovered that it was making an unrealistic assumption: growers want to provide enough supplemental light to reach their target DLI _every single day of the year_. Because of that unrealistic assumption, I decided not to calculate demand charges and begin working on two new calculators (SupplementalCalc and TargetCalc).

**Description:** LightingCalc was created to determine how much electricity is required to reach the target DLI every single day of the year. To do so, a lighting system would need to be designed to provide enough light on even the darkest day of the year. On the Electricity Cost page, users will view a dashboard that calculates lighting costs at an annual, monthly, and weekly view.


### SupplementalCalc
[![](https://img.shields.io/badge/ShinyApps.io-Open_Web_App-3686d3?logo=r)](https://3dcxni-jarryd-wannenburg.shinyapps.io/SupplementalCalc/) 
[![](https://img.shields.io/badge/GitHub-View_on_GitHub-6e5494?logo=GitHub)](https://github.com/JarrydWannenburg/SupplementalCalc)
[![](https://img.shields.io/badge/YouTube-Watch_User_Walkthrough-FF0000?logo=YouTube)](https://youtu.be/TTYsi2jaqUw)

**Concepts:** APIs, Data Transformation, Data Analytics, Data Visualization, Interactive Web App Development

**Skills:** R (shiny, dyplr, ggplot2, lubridate, tidygeocoder)

**Background:** After realizing the unrealistic assumption made in LightingCalc, I set out to build a new calculator that relaxed that assumption. The result was a web application that allows a user to specify what percent of the year they'd like to reach their target DLI and how many hours they light their greenhouse. I also rebuilt the dashboard to calculate demand charges and visualize a scatterplot of the amount of sunlight coming into the greenhouse and how much supplemental light is needed.

**Description:** SupplementalCalc was created to determine how much electricity is required to reach the target DLI given what percent of the year the user wants to reach that target and how many hours their lights are on per day. On the Electricity Cost page, users will view a dashboard that calculates lighting costs at an annual, monthly, and weekly view. The page components are dynamic and change to the user's mouse click on the scatterplot, which represents changing the percentile of days and makes this the most advanced calculator of the three.


### TargetCalc
[![](https://img.shields.io/badge/ShinyApps.io-Open_Web_App-3686d3?logo=r)](https://3dcxni-jarryd-wannenburg.shinyapps.io/TargetCalc/)
[![](https://img.shields.io/badge/GitHub-View_on_GitHub-6e5494?logo=GitHub)](https://github.com/JarrydWannenburg/TargetCalc)
[![](https://img.shields.io/badge/YouTube-Watch_User_Walkthrough-FF0000?logo=YouTube)](https://youtu.be/0VDcWBuC4rY)

**Concepts:** APIs, Data Transformation, Data Analytics, Data Visualization, Web App Development

**Skills:** R (shiny, dyplr, ggplot2, lubridate, tidygeocoder)

**Background:** Once I had finished building SupplementalCalc, the LAMP agricultral team came to me with a request to build a third calculator that would output what percent of the year a greenhouse grower could expect to reach their target DLI given inputs describing a lighting system currently in place. 

**Description:** With TargetCalc, users specify the capacity of their lighting system, and the calculator will estimate on how many days of the year you can reach your target DLI. The associated electricity costs and demand charge are estimated as well. This calculator is particularly useful for determining how well an existing lighting system meets your needs.


### SolarPanelEstimator_one
[![](https://img.shields.io/badge/ShinyApps.io-Open_Web_App-3686d3?logo=r)](https://3dcxni-jarryd-wannenburg.shinyapps.io/SolarPanelEstimator_one/)
[![](https://img.shields.io/badge/GitHub-View_on_GitHub-6e5494?logo=GitHub)](https://github.com/JarrydWannenburg/SolarPanelEstimator_one)
[![](https://img.shields.io/badge/YouTube-Watch_User_Walkthrough-FF0000?logo=YouTube)]()

**Concepts:** APIs, Data Transformation, Data Analytics, Data Visualization, Web App Development

**Skills:** R (shiny, dyplr, ggplot2, lubridate, tidygeocoder)

**Background:** After completing the previous three calculators, I still had a few months until graduation, so I was asked to try build a solar panel estimator that optimizes the number of panels to install by minimizing the total cost, which breaks down into capital cost, installation cost, and grid purchase costs. The first attempt produced the SolarPanelEstimator_one. _This version of the estimator is what I had finished by the end of my assistantship (May 2022), so a few bugs may remain_.

**Description:** With this estimator, users specify details of a solar panel system, and the calculator will estimate the optimal number of panels to install by minimizing the electricity cost for a given location. The single period optimization doesn't recognize rising costs when optimizing, which led to the creation of the multi period version of this calculator. The associated grid purchase costs and generated electricity are estimated as well. This calculator is useful when looking to install a solar system, but users should default to the multi period version.


### SolarPanelEstimator_multi 
[![](https://img.shields.io/badge/ShinyApps.io-Open_Web_App-3686d3?logo=r)](https://3dcxni-jarryd-wannenburg.shinyapps.io/SolarPanelEstimator_multi/)
[![](https://img.shields.io/badge/GitHub-View_on_GitHub-6e5494?logo=GitHub)](https://github.com/JarrydWannenburg/SolarPanelEstimator_multi)
[![](https://img.shields.io/badge/YouTube-Watch_User_Walkthrough-FF0000?logo=YouTube)]()

**Concepts:** APIs, Data Transformation, Data Analytics, Data Visualization, Web App Development

**Skills:** R (shiny, dyplr, ggplot2, lubridate, tidygeocoder)

**Background:** The second attempt at minimizing cost (capital cost + installation cost + grid purchase cost) approached the problem with multi period integer optimizations, producing the SolarPanelEstimator_multi. A cost effective interpretation of the results of this estimator would be to install the framework for the optimal number of panels in the first period. Then, as the estimator adds panels to the calculation, panels should be purchased and added to the existing framework to reduce installation costs. _This version of the estimator is what I had finished by the end of my assistantship (May 2022), so a few bugs may remain_.

**Description:** With this estimator, users can specify detailed information of a solar panel system of interest or use default values provided by the National Renewable Energy Laboratory (NREL). After entering information specific to the solar panels and selecting the preferred datasource, the estimator will provide a breakdown of energy costs and outputs expected by using these solar panels. This estimator also estimates the optimal number of panels needed to meet a user's specified annual energy demand. This estimator is particularly useful for the design of new solar panel installations. 
